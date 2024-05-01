# Comparing `tmp/sentient_switchblade-0.3.5.tar.gz` & `tmp/sentient_switchblade-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentient_switchblade-0.3.5.tar", max compression
+gzip compressed data, was "sentient_switchblade-0.3.6.tar", max compression
```

## Comparing `sentient_switchblade-0.3.5.tar` & `sentient_switchblade-0.3.6.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1077 2023-04-25 19:36:38.976660 sentient_switchblade-0.3.5/LICENSE
--rw-r--r--   0        0        0     8451 2023-05-05 21:59:38.933062 sentient_switchblade-0.3.5/README.md
--rw-r--r--   0        0        0     1752 2023-05-05 22:16:23.143228 sentient_switchblade-0.3.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 19:36:27.260808 sentient_switchblade-0.3.5/src/switchbladecli/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 19:35:52.447291 sentient_switchblade-0.3.5/src/switchbladecli/cli/__init__.py
--rw-r--r--   0        0        0     1491 2023-05-04 19:17:19.432214 sentient_switchblade-0.3.5/src/switchbladecli/cli/__main__.py
--rw-r--r--   0        0        0    11546 2023-05-05 22:01:56.410802 sentient_switchblade-0.3.5/src/switchbladecli/cli/bundle_cache.py
--rw-r--r--   0        0        0     1725 2023-05-01 18:05:13.432197 sentient_switchblade-0.3.5/src/switchbladecli/cli/config.py
--rw-r--r--   0        0        0      734 2023-05-05 20:07:43.738620 sentient_switchblade-0.3.5/src/switchbladecli/cli/lint.py
--rw-r--r--   0        0        0      740 2023-05-05 20:08:11.028589 sentient_switchblade-0.3.5/src/switchbladecli/cli/test.py
--rw-r--r--   0        0        0      479 2023-05-04 20:41:51.180130 sentient_switchblade-0.3.5/src/switchbladecli/cli/update.py
--rw-r--r--   0        0        0      256 2023-05-04 22:00:04.840133 sentient_switchblade-0.3.5/src/switchbladecli/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-26 17:36:55.033765 sentient_switchblade-0.3.5/src/switchbladecli/modes/__init__.py
--rw-r--r--   0        0        0    11861 2023-05-05 20:24:32.708701 sentient_switchblade-0.3.5/src/switchbladecli/modes/python_poetry.py
--rw-r--r--   0        0        0      415 2023-05-04 22:00:19.685629 sentient_switchblade-0.3.5/src/switchbladecli/modes/tool_runner.py
--rw-r--r--   0        0        0      848 2023-05-04 21:04:15.624544 sentient_switchblade-0.3.5/src/switchbladecli/utils.py
--rw-r--r--   0        0        0     9663 1970-01-01 00:00:00.000000 sentient_switchblade-0.3.5/setup.py
--rw-r--r--   0        0        0     9807 1970-01-01 00:00:00.000000 sentient_switchblade-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-25 19:36:38.976660 sentient_switchblade-0.3.6/LICENSE
+-rw-r--r--   0        0        0     8451 2023-05-05 21:59:38.933062 sentient_switchblade-0.3.6/README.md
+-rw-r--r--   0        0        0     1828 2024-05-01 22:01:28.690190 sentient_switchblade-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 19:36:27.260808 sentient_switchblade-0.3.6/src/switchbladecli/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 19:35:52.447291 sentient_switchblade-0.3.6/src/switchbladecli/cli/__init__.py
+-rw-r--r--   0        0        0     1491 2023-05-04 19:17:19.432214 sentient_switchblade-0.3.6/src/switchbladecli/cli/__main__.py
+-rw-r--r--   0        0        0    11531 2024-05-01 21:33:43.406591 sentient_switchblade-0.3.6/src/switchbladecli/cli/bundle_cache.py
+-rw-r--r--   0        0        0     1725 2023-05-01 18:05:13.432197 sentient_switchblade-0.3.6/src/switchbladecli/cli/config.py
+-rw-r--r--   0        0        0      734 2023-05-05 20:07:43.738620 sentient_switchblade-0.3.6/src/switchbladecli/cli/lint.py
+-rw-r--r--   0        0        0      740 2023-05-05 20:08:11.028589 sentient_switchblade-0.3.6/src/switchbladecli/cli/test.py
+-rw-r--r--   0        0        0      479 2023-05-04 20:41:51.180130 sentient_switchblade-0.3.6/src/switchbladecli/cli/update.py
+-rw-r--r--   0        0        0      256 2023-05-04 22:00:04.840133 sentient_switchblade-0.3.6/src/switchbladecli/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-26 17:36:55.033765 sentient_switchblade-0.3.6/src/switchbladecli/modes/__init__.py
+-rw-r--r--   0        0        0    11861 2023-05-05 20:24:32.708701 sentient_switchblade-0.3.6/src/switchbladecli/modes/python_poetry.py
+-rw-r--r--   0        0        0      415 2023-05-04 22:00:19.685629 sentient_switchblade-0.3.6/src/switchbladecli/modes/tool_runner.py
+-rw-r--r--   0        0        0      848 2023-05-04 21:04:15.624544 sentient_switchblade-0.3.6/src/switchbladecli/utils.py
+-rw-r--r--   0        0        0     9610 1970-01-01 00:00:00.000000 sentient_switchblade-0.3.6/PKG-INFO
```

### Comparing `sentient_switchblade-0.3.5/LICENSE` & `sentient_switchblade-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.3.5/README.md` & `sentient_switchblade-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.3.5/pyproject.toml` & `sentient_switchblade-0.3.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sentient-switchblade"
-version = "0.3.5"
+version = "0.3.6"
 description = "Unleash Dev Tool Mastery with a Flick of Your Wrist"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/sentient-switchblade"
 homepage = "https://jensroland.com/sentient-switchblade"
 readme = "README.md"
 packages = [
@@ -17,35 +17,37 @@
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
 
 [tool.poetry.scripts]
 swb = "switchbladecli.cli.__main__:switchbladecli"
 
 [tool.poetry.dependencies]
 checksumdir = "^1.2.0"
 click = "^8.0.3"
 mergedeep = "^1.3.4"
 PyGithub = "^1.58.1"
-python = "^3.7"
+python = "^3.8"
 tomlkit = "^0.11.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
 pytest-subprocess = "^1.5.0"
 tox = "^4.5.1"
+virtualenv-pyenv = "^0.5.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 # Directories that are not visited by pytest collector:
```

### Comparing `sentient_switchblade-0.3.5/src/switchbladecli/cli/__main__.py` & `sentient_switchblade-0.3.6/src/switchbladecli/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.3.5/src/switchbladecli/cli/bundle_cache.py` & `sentient_switchblade-0.3.6/src/switchbladecli/cli/bundle_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import click
 import os
 import shutil
 
 from datetime import datetime, timezone
-from distutils.dir_util import copy_tree
 from github import Github
 from mergedeep import merge
 from pathlib import Path
 from tomlkit import dumps, loads
 
 from switchbladecli.utils import hash_dir
 
@@ -135,15 +134,15 @@
             # Download all the files
             for repo_asset in repo_contents:
                 with open(bundle_folder / repo_asset.name, "wb") as file:
                     file.write(repo_asset.decoded_content)
 
         else:
             # If the source is a local folder, copy it to the cache
-            copy_tree(str(bundle_source_uri), str(bundle_folder))
+            shutil.copytree(str(bundle_source_uri), str(bundle_folder), dirs_exist_ok=True)
 
         cache.log(f"UPDATING {remote_version} SUCCEEDED")
 
         new_bundle = Bundle(self._switchblade_config, remote_version)
         cache.set_latest_config(new_bundle)
 
         # Finally, return the fetched bundle
```

### Comparing `sentient_switchblade-0.3.5/src/switchbladecli/cli/config.py` & `sentient_switchblade-0.3.6/src/switchbladecli/cli/config.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.3.5/src/switchbladecli/cli/lint.py` & `sentient_switchblade-0.3.6/src/switchbladecli/cli/lint.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.3.5/src/switchbladecli/cli/test.py` & `sentient_switchblade-0.3.6/src/switchbladecli/cli/test.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.3.5/src/switchbladecli/modes/python_poetry.py` & `sentient_switchblade-0.3.6/src/switchbladecli/modes/python_poetry.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.3.5/src/switchbladecli/utils.py` & `sentient_switchblade-0.3.6/src/switchbladecli/utils.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.3.5/setup.py` & `sentient_switchblade-0.3.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,187 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sentient-switchblade
+Version: 0.3.6
+Summary: Unleash Dev Tool Mastery with a Flick of Your Wrist
+Home-page: https://jensroland.com/sentient-switchblade
+License: MIT
+Author: JensRoland
+Author-email: mail@jensroland.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: PyGithub (>=1.58.1,<2.0.0)
+Requires-Dist: checksumdir (>=1.2.0,<2.0.0)
+Requires-Dist: click (>=8.0.3,<9.0.0)
+Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
+Requires-Dist: tomlkit (>=0.11.7,<0.12.0)
+Project-URL: Repository, https://github.com/jensroland/sentient-switchblade
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->
+<p align="center">
+  <a href="https://github.com/JensRoland/sentient-switchblade">
+    <img src="https://jensroland.com/switchblade/assets/switchblade-logotype.png" width="415px" alt="Switchblade logo" />
+  </a>
+</p>
 
-packages = \
-['switchbladecli', 'switchbladecli.cli', 'switchbladecli.modes']
+<h3 align="center">Unleash Dev Tool Mastery with a Flick of Your Wrist</h3>
+<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a></p>
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyGithub>=1.58.1,<2.0.0',
- 'checksumdir>=1.2.0,<2.0.0',
- 'click>=8.0.3,<9.0.0',
- 'mergedeep>=1.3.4,<2.0.0',
- 'tomlkit>=0.11.7,<0.12.0']
-
-entry_points = \
-{'console_scripts': ['swb = switchbladecli.cli.__main__:switchbladecli']}
-
-setup_kwargs = {
-    'name': 'sentient-switchblade',
-    'version': '0.3.5',
-    'description': 'Unleash Dev Tool Mastery with a Flick of Your Wrist',
-    'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://github.com/JensRoland/sentient-switchblade">\n    <img src="https://jensroland.com/switchblade/assets/switchblade-logotype.png" width="415px" alt="Switchblade logo" />\n  </a>\n</p>\n\n<h3 align="center">Unleash Dev Tool Mastery with a Flick of Your Wrist</h3>\n<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a></p>\n\n<br />\n\n## ⚔️ What is Switchblade?\n\nSwitchblade is a command line tool that lets you install and run dev tools from a central repository, and configure them in a standardised way across all your projects.\n\n## Try it\n\nTo use the included `python-poetry-base` bundle for Python, create a `.switchblade` file in your project root:\n\n```toml\n[switchblade]\nbundle = "gh:jensroland/sentient-switchblade/bundles/python-poetry-base"\nmode = "python-poetry"\n```\n\nThen, install Switchblade in your project and call `swb lint` to run the standard Python linters configured in the base bundle:\n\n```shell\n# Install Switchblade\npoetry add -G dev sentient-switchblade\n\n# Run linters from the bundle\npoetry run swb lint\n```\n\nThat\'s it! :tada: Switchblade will fetch the bundle from Github, install the tools specified in the bundle, and run them with the configurations specified in the bundle. No need to install or configure anything yourself, and no need to commit any dev tooling to your project repo.\n\n**Note**: The base bundle assumes that your source code lives under `src/` and your tests under `tests/`, but it is only meant as an example. To specify your own dev tools and tailor them to your needs and project structure, create your own custom bundle (see below).\n\n## Who is this for?\n\nSwitchblade was born from the question: *"How do I ensure that I\'m using the same linting and testing configurations across all of my project repositories?"* Are all of your Python repos using the same version of `Black`? Maybe you switched to `flake8` on your newer repos but never updated the old ones? Sure, maybe it doesn\'t matter very much if your tooling deviates a little between your personal projects, but how about this: when your company\'s DevSecOps team updated all the templates to include scans for known vulnerabilities and credential leaks, did you remember to update all of your repos? And if not, how would you even know?\n\nTo complicate matters, developer tooling is not simply about choosing a particular linter and firing it up. It\'s also how you configure it -- maximum line lengths, whether to use single or double quotes, what rules to ignore entirely -- as well as which arguments to pass when you invoke it.\n\n<!-- Every software engineering organisation has to deal with these issues, and while many solutions exist, they are hardly perfect:\n\n1. Provide project templates with dev tooling built-in, and use those templates to create new projects. This works well initially, but results in duplicated configuration files and makes all subsequent configuration updates both time consuming and error prone, since they have to be made in all projects at once.\n2. Let configs be duplicated across projects and use [a meta-repo tool](https://github.com/mateodelnorte/meta) to perform cross-repo updates. This requires a non-trivial amount of setup and maintenance, and updating a dev configuration still requires committing changes in every repo.\n3. Combine all dev tooling in a package and install it in every project. This works for some types of tooling, but many tools require their config files to exist in the project root rather than inside a package. It also usually requires committing changes (e.g. the updated lockfile) in every repo to get the latest configurations.\n4. Use a monorepo; have one set of dev tools included in the repo and use it for everything. This can actually be a great solution, but it\'s not always possible or desirable to use a monorepo.\n5. Something custom involving Docker containers and prebaked images with dev tools. This involves a lot of complexity and overhead, plus you get all the limitations of the package solution. -->\n\nIn an ideal world, dev tooling would not be checked into version control (*seriously*) but rather **fetched on demand from a centrally managed dev tooling repository, and configured and invoked in exactly the same way in every repo, every time**. This would allow for a single source of truth for all dev tooling, and would make it easy to update configurations across all projects.\n\nTo achieve this however, you would need some kind of small helper tool to abstract away the fetching, configuring and invoking of your centrally curated \'bundles\' of dev tools.\n\nSwitchblade is that tool.\n\n## Custom bundles\n\nTo create your own custom bundle with the dev tools and configurations you need, simply create a new Github repo and add a `bundle.toml` file to it:\n\n```toml\n[bundle]\nname = "my-dev-tool-bundle"\nmode = "python-poetry"\nschema_version = "1.0.0"\n\n# Linters\n[linters]\nall = ["pylint"]\n\n[linters.pylint]\ncommand = "pylint src"\n\n# Tests\n[tests]\nall = ["pytest"]\n\n[tests.pytest]\ncommand = "pytest -c pyproject.toml tests"\n\n# Extensions to pyproject.toml\n[tool.poetry.group.switchblade]\noptional = true\n\n[tool.poetry.group.switchblade.dependencies]\npylint = "^2.17.2"\npytest = "^7.3.1"\n\n[tool.pytest.ini_options]\npythonpath = "src"\n```\n\nFor each linter you want to add, specify a `[linters.<toolname>]` section with a `command` key. The `command` value will be invoked by Switchblade when you run `swb lint <toolname>`.\n\nThe `[linters]` section specifies which linters should be invoked (and in which order) when you run `swb lint` or `swb lint all`.\n\nThe same goes for tests: specify a `[tests.<toolname>]` section with a `command` key, and add the tool to the `[tests]` section to have it invoked when you run `swb test` or `swb test all`.\n\n### Tool configuration\n\nAnything in the `bundle.toml` file under a `tool.*` section will be temporarily added to the project\'s `pyproject.toml` file under that section. This allows you to add dependencies and configuration options to all your projects without having to manually edit all the individual `pyproject.toml` files.\n\nIf you prefer having separate config files, or for tools which do not support `pyproject.toml` configuration, simply add any config files you need in the same folder as the `bundle.toml` file. E.g. you might define a `.pylintrc` in the bundle repo:\n\n```ini\n[MAIN]\n[MESSAGES CONTROL]\ndisable=\n    C0111,  # missing-docstring\n    C0114,  # missing-module-docstring\n    C0115,  # missing-class-docstring\n    C0116,  # missing-function-docstring\n    W0613,  # unused-argument\n```\n\nNow, when you want to use your custom dev tool bundle in a project, simply point to the repo in the project `.switchblade` file as in the example above. Swichblade will then fetch and install the tools you specified in the bundle and run them with the configurations you specified.\n\n### Per-project overrides\n\nTo override the bundle configuration for a specific dev tool in one of your project repos, simply check in the tool dependencies and configuration files in the project repo as you normally would - Switchblade will still invoke the dev tool, but it will not overwrite any existing config files or `[tool.*]` sections in your `pyproject.toml` file. Be aware that this does not \'extend\' the configuration from the bundle, but replaces that tool configuration entirely, so this feature should be used with caution.\n\nTo override the command or the list of linters to run, add the corresponding sections (e.g. `[linters]` or `[linters.pylint]` in the project `.switchblade` file. Switchblade will automatically merge (in this case it does extend rather than replace) the bundle config and Switchblade config before invoking any of the tools.\n\n## Prerequisites\n\n- [Python 3.7+](https://www.python.org/downloads/)\n\nCurrently, you need Python since you install Switchblade with pip. This may change in the future.\n\n## Features\n\n- CLI command `swb lint` to run linters\n- CLI command `swb test` to run tests\n- Project \'modes\' supported: Currently only `python-poetry` is supported, but more will be added soon.\n\n## Development\n\nInstall dependencies:\n\n```shell\n> poetry install\n```\n\nRun unit tests with coverage:\n\n```shell\n> poetry run pytest -c pyproject.toml --cov-report=term --cov=src tests\n```\n\nOr run unit tests on multiple Python versions with tox:\n\n```shell\n> poetry run tox\n```\n',
-    'author': 'JensRoland',
-    'author_email': 'mail@jensroland.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://jensroland.com/sentient-switchblade',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+<br />
 
+## ⚔️ What is Switchblade?
+
+Switchblade is a command line tool that lets you install and run dev tools from a central repository, and configure them in a standardised way across all your projects.
+
+## Try it
+
+To use the included `python-poetry-base` bundle for Python, create a `.switchblade` file in your project root:
+
+```toml
+[switchblade]
+bundle = "gh:jensroland/sentient-switchblade/bundles/python-poetry-base"
+mode = "python-poetry"
+```
+
+Then, install Switchblade in your project and call `swb lint` to run the standard Python linters configured in the base bundle:
+
+```shell
+# Install Switchblade
+poetry add -G dev sentient-switchblade
+
+# Run linters from the bundle
+poetry run swb lint
+```
+
+That's it! :tada: Switchblade will fetch the bundle from Github, install the tools specified in the bundle, and run them with the configurations specified in the bundle. No need to install or configure anything yourself, and no need to commit any dev tooling to your project repo.
+
+**Note**: The base bundle assumes that your source code lives under `src/` and your tests under `tests/`, but it is only meant as an example. To specify your own dev tools and tailor them to your needs and project structure, create your own custom bundle (see below).
+
+## Who is this for?
+
+Switchblade was born from the question: *"How do I ensure that I'm using the same linting and testing configurations across all of my project repositories?"* Are all of your Python repos using the same version of `Black`? Maybe you switched to `flake8` on your newer repos but never updated the old ones? Sure, maybe it doesn't matter very much if your tooling deviates a little between your personal projects, but how about this: when your company's DevSecOps team updated all the templates to include scans for known vulnerabilities and credential leaks, did you remember to update all of your repos? And if not, how would you even know?
+
+To complicate matters, developer tooling is not simply about choosing a particular linter and firing it up. It's also how you configure it -- maximum line lengths, whether to use single or double quotes, what rules to ignore entirely -- as well as which arguments to pass when you invoke it.
+
+<!-- Every software engineering organisation has to deal with these issues, and while many solutions exist, they are hardly perfect:
+
+1. Provide project templates with dev tooling built-in, and use those templates to create new projects. This works well initially, but results in duplicated configuration files and makes all subsequent configuration updates both time consuming and error prone, since they have to be made in all projects at once.
+2. Let configs be duplicated across projects and use [a meta-repo tool](https://github.com/mateodelnorte/meta) to perform cross-repo updates. This requires a non-trivial amount of setup and maintenance, and updating a dev configuration still requires committing changes in every repo.
+3. Combine all dev tooling in a package and install it in every project. This works for some types of tooling, but many tools require their config files to exist in the project root rather than inside a package. It also usually requires committing changes (e.g. the updated lockfile) in every repo to get the latest configurations.
+4. Use a monorepo; have one set of dev tools included in the repo and use it for everything. This can actually be a great solution, but it's not always possible or desirable to use a monorepo.
+5. Something custom involving Docker containers and prebaked images with dev tools. This involves a lot of complexity and overhead, plus you get all the limitations of the package solution. -->
+
+In an ideal world, dev tooling would not be checked into version control (*seriously*) but rather **fetched on demand from a centrally managed dev tooling repository, and configured and invoked in exactly the same way in every repo, every time**. This would allow for a single source of truth for all dev tooling, and would make it easy to update configurations across all projects.
+
+To achieve this however, you would need some kind of small helper tool to abstract away the fetching, configuring and invoking of your centrally curated 'bundles' of dev tools.
+
+Switchblade is that tool.
+
+## Custom bundles
+
+To create your own custom bundle with the dev tools and configurations you need, simply create a new Github repo and add a `bundle.toml` file to it:
+
+```toml
+[bundle]
+name = "my-dev-tool-bundle"
+mode = "python-poetry"
+schema_version = "1.0.0"
+
+# Linters
+[linters]
+all = ["pylint"]
+
+[linters.pylint]
+command = "pylint src"
+
+# Tests
+[tests]
+all = ["pytest"]
+
+[tests.pytest]
+command = "pytest -c pyproject.toml tests"
+
+# Extensions to pyproject.toml
+[tool.poetry.group.switchblade]
+optional = true
+
+[tool.poetry.group.switchblade.dependencies]
+pylint = "^2.17.2"
+pytest = "^7.3.1"
+
+[tool.pytest.ini_options]
+pythonpath = "src"
+```
+
+For each linter you want to add, specify a `[linters.<toolname>]` section with a `command` key. The `command` value will be invoked by Switchblade when you run `swb lint <toolname>`.
+
+The `[linters]` section specifies which linters should be invoked (and in which order) when you run `swb lint` or `swb lint all`.
+
+The same goes for tests: specify a `[tests.<toolname>]` section with a `command` key, and add the tool to the `[tests]` section to have it invoked when you run `swb test` or `swb test all`.
+
+### Tool configuration
+
+Anything in the `bundle.toml` file under a `tool.*` section will be temporarily added to the project's `pyproject.toml` file under that section. This allows you to add dependencies and configuration options to all your projects without having to manually edit all the individual `pyproject.toml` files.
+
+If you prefer having separate config files, or for tools which do not support `pyproject.toml` configuration, simply add any config files you need in the same folder as the `bundle.toml` file. E.g. you might define a `.pylintrc` in the bundle repo:
+
+```ini
+[MAIN]
+[MESSAGES CONTROL]
+disable=
+    C0111,  # missing-docstring
+    C0114,  # missing-module-docstring
+    C0115,  # missing-class-docstring
+    C0116,  # missing-function-docstring
+    W0613,  # unused-argument
+```
+
+Now, when you want to use your custom dev tool bundle in a project, simply point to the repo in the project `.switchblade` file as in the example above. Swichblade will then fetch and install the tools you specified in the bundle and run them with the configurations you specified.
+
+### Per-project overrides
+
+To override the bundle configuration for a specific dev tool in one of your project repos, simply check in the tool dependencies and configuration files in the project repo as you normally would - Switchblade will still invoke the dev tool, but it will not overwrite any existing config files or `[tool.*]` sections in your `pyproject.toml` file. Be aware that this does not 'extend' the configuration from the bundle, but replaces that tool configuration entirely, so this feature should be used with caution.
+
+To override the command or the list of linters to run, add the corresponding sections (e.g. `[linters]` or `[linters.pylint]` in the project `.switchblade` file. Switchblade will automatically merge (in this case it does extend rather than replace) the bundle config and Switchblade config before invoking any of the tools.
+
+## Prerequisites
+
+- [Python 3.7+](https://www.python.org/downloads/)
+
+Currently, you need Python since you install Switchblade with pip. This may change in the future.
+
+## Features
+
+- CLI command `swb lint` to run linters
+- CLI command `swb test` to run tests
+- Project 'modes' supported: Currently only `python-poetry` is supported, but more will be added soon.
+
+## Development
+
+Install dependencies:
+
+```shell
+> poetry install
+```
+
+Run unit tests with coverage:
+
+```shell
+> poetry run pytest -c pyproject.toml --cov-report=term --cov=src tests
+```
+
+Or run unit tests on multiple Python versions with tox:
+
+```shell
+> poetry run tox
+```
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,108 +1,104 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['switchbladecli', 'switchbladecli.cli',
-'switchbladecli.modes'] package_data = \ {'': ['*']} install_requires = \
-['PyGithub>=1.58.1,<2.0.0', 'checksumdir>=1.2.0,<2.0.0', 'click>=8.0.3,<9.0.0',
-'mergedeep>=1.3.4,<2.0.0', 'tomlkit>=0.11.7,<0.12.0'] entry_points = \
-{'console_scripts': ['swb = switchbladecli.cli.__main__:switchbladecli']}
-setup_kwargs = { 'name': 'sentient-switchblade', 'version': '0.3.5',
-'description': 'Unleash Dev Tool Mastery with a Flick of Your Wrist',
-'long_description': '\n
-                         \n _\_n_ _[_S_w_i_t_c_h_b_l_a_d_e_ _l_o_g_o_]_\_n_ \n
-\n\n
+Metadata-Version: 2.1 Name: sentient-switchblade Version: 0.3.6 Summary:
+Unleash Dev Tool Mastery with a Flick of Your Wrist Home-page: https://
+jensroland.com/sentient-switchblade License: MIT Author: JensRoland Author-
+email: mail@jensroland.com Requires-Python: >=3.8,<4.0 Classifier: Development
+Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Dist: PyGithub (>=1.58.1,<2.0.0) Requires-Dist: checksumdir
+(>=1.2.0,<2.0.0) Requires-Dist: click (>=8.0.3,<9.0.0) Requires-Dist: mergedeep
+(>=1.3.4,<2.0.0) Requires-Dist: tomlkit (>=0.11.7,<0.12.0) Project-URL:
+Repository, https://github.com/jensroland/sentient-switchblade Description-
+Content-Type: text/markdown
+                              _[_S_w_i_t_c_h_b_l_a_d_e_ _l_o_g_o_]
          ******** UUnnlleeaasshh DDeevv TTooooll MMaasstteerryy wwiitthh aa FFlliicckk ooff YYoouurr WWrriisstt ********
-\n
                             Created by _J_e_n_s_ _R_o_l_a_n_d
-\n\n
-\n\n## âï¸ What is Switchblade?\n\nSwitchblade is a command line tool that
-lets you install and run dev tools from a central repository, and configure
-them in a standardised way across all your projects.\n\n## Try it\n\nTo use the
-included `python-poetry-base` bundle for Python, create a `.switchblade` file
-in your project root:\n\n```toml\n[switchblade]\nbundle = "gh:jensroland/
-sentient-switchblade/bundles/python-poetry-base"\nmode = "python-
-poetry"\n```\n\nThen, install Switchblade in your project and call `swb lint`
-to run the standard Python linters configured in the base bundle:
-\n\n```shell\n# Install Switchblade\npoetry add -G dev sentient-
-switchblade\n\n# Run linters from the bundle\npoetry run swb
-lint\n```\n\nThat\'s it! :tada: Switchblade will fetch the bundle from Github,
+
+## âï¸ What is Switchblade? Switchblade is a command line tool that lets you
+install and run dev tools from a central repository, and configure them in a
+standardised way across all your projects. ## Try it To use the included
+`python-poetry-base` bundle for Python, create a `.switchblade` file in your
+project root: ```toml [switchblade] bundle = "gh:jensroland/sentient-
+switchblade/bundles/python-poetry-base" mode = "python-poetry" ``` Then,
+install Switchblade in your project and call `swb lint` to run the standard
+Python linters configured in the base bundle: ```shell # Install Switchblade
+poetry add -G dev sentient-switchblade # Run linters from the bundle poetry run
+swb lint ``` That's it! :tada: Switchblade will fetch the bundle from Github,
 install the tools specified in the bundle, and run them with the configurations
 specified in the bundle. No need to install or configure anything yourself, and
-no need to commit any dev tooling to your project repo.\n\n**Note**: The base
+no need to commit any dev tooling to your project repo. **Note**: The base
 bundle assumes that your source code lives under `src/` and your tests under
 `tests/`, but it is only meant as an example. To specify your own dev tools and
 tailor them to your needs and project structure, create your own custom bundle
-(see below).\n\n## Who is this for?\n\nSwitchblade was born from the question:
-*"How do I ensure that I\'m using the same linting and testing configurations
-across all of my project repositories?"* Are all of your Python repos using the
-same version of `Black`? Maybe you switched to `flake8` on your newer repos but
-never updated the old ones? Sure, maybe it doesn\'t matter very much if your
+(see below). ## Who is this for? Switchblade was born from the question: *"How
+do I ensure that I'm using the same linting and testing configurations across
+all of my project repositories?"* Are all of your Python repos using the same
+version of `Black`? Maybe you switched to `flake8` on your newer repos but
+never updated the old ones? Sure, maybe it doesn't matter very much if your
 tooling deviates a little between your personal projects, but how about this:
-when your company\'s DevSecOps team updated all the templates to include scans
+when your company's DevSecOps team updated all the templates to include scans
 for known vulnerabilities and credential leaks, did you remember to update all
-of your repos? And if not, how would you even know?\n\nTo complicate matters,
+of your repos? And if not, how would you even know? To complicate matters,
 developer tooling is not simply about choosing a particular linter and firing
-it up. It\'s also how you configure it -- maximum line lengths, whether to use
+it up. It's also how you configure it -- maximum line lengths, whether to use
 single or double quotes, what rules to ignore entirely -- as well as which
-arguments to pass when you invoke it.\n\n\n\nIn an ideal world, dev tooling
-would not be checked into version control (*seriously*) but rather **fetched on
-demand from a centrally managed dev tooling repository, and configured and
-invoked in exactly the same way in every repo, every time**. This would allow
-for a single source of truth for all dev tooling, and would make it easy to
-update configurations across all projects.\n\nTo achieve this however, you
-would need some kind of small helper tool to abstract away the fetching,
-configuring and invoking of your centrally curated \'bundles\' of dev
-tools.\n\nSwitchblade is that tool.\n\n## Custom bundles\n\nTo create your own
-custom bundle with the dev tools and configurations you need, simply create a
-new Github repo and add a `bundle.toml` file to it:\n\n```toml\n[bundle]\nname
-= "my-dev-tool-bundle"\nmode = "python-poetry"\nschema_version = "1.0.0"\n\n#
-Linters\n[linters]\nall = ["pylint"]\n\n[linters.pylint]\ncommand = "pylint
-src"\n\n# Tests\n[tests]\nall = ["pytest"]\n\n[tests.pytest]\ncommand = "pytest
--c pyproject.toml tests"\n\n# Extensions to pyproject.toml\n
-[tool.poetry.group.switchblade]\noptional = true\n\n
-[tool.poetry.group.switchblade.dependencies]\npylint = "^2.17.2"\npytest =
-"^7.3.1"\n\n[tool.pytest.ini_options]\npythonpath = "src"\n```\n\nFor each
-linter you want to add, specify a `[linters.]` section with a `command` key.
-The `command` value will be invoked by Switchblade when you run `swb lint
-`.\n\nThe `[linters]` section specifies which linters should be invoked (and in
-which order) when you run `swb lint` or `swb lint all`.\n\nThe same goes for
-tests: specify a `[tests.]` section with a `command` key, and add the tool to
-the `[tests]` section to have it invoked when you run `swb test` or `swb test
-all`.\n\n### Tool configuration\n\nAnything in the `bundle.toml` file under a
-`tool.*` section will be temporarily added to the project\'s `pyproject.toml`
-file under that section. This allows you to add dependencies and configuration
-options to all your projects without having to manually edit all the individual
-`pyproject.toml` files.\n\nIf you prefer having separate config files, or for
-tools which do not support `pyproject.toml` configuration, simply add any
-config files you need in the same folder as the `bundle.toml` file. E.g. you
-might define a `.pylintrc` in the bundle repo:\n\n```ini\n[MAIN]\n[MESSAGES
-CONTROL]\ndisable=\n C0111, # missing-docstring\n C0114, # missing-module-
-docstring\n C0115, # missing-class-docstring\n C0116, # missing-function-
-docstring\n W0613, # unused-argument\n```\n\nNow, when you want to use your
-custom dev tool bundle in a project, simply point to the repo in the project
-`.switchblade` file as in the example above. Swichblade will then fetch and
-install the tools you specified in the bundle and run them with the
-configurations you specified.\n\n### Per-project overrides\n\nTo override the
+arguments to pass when you invoke it. In an ideal world, dev tooling would not
+be checked into version control (*seriously*) but rather **fetched on demand
+from a centrally managed dev tooling repository, and configured and invoked in
+exactly the same way in every repo, every time**. This would allow for a single
+source of truth for all dev tooling, and would make it easy to update
+configurations across all projects. To achieve this however, you would need
+some kind of small helper tool to abstract away the fetching, configuring and
+invoking of your centrally curated 'bundles' of dev tools. Switchblade is that
+tool. ## Custom bundles To create your own custom bundle with the dev tools and
+configurations you need, simply create a new Github repo and add a
+`bundle.toml` file to it: ```toml [bundle] name = "my-dev-tool-bundle" mode =
+"python-poetry" schema_version = "1.0.0" # Linters [linters] all = ["pylint"]
+[linters.pylint] command = "pylint src" # Tests [tests] all = ["pytest"]
+[tests.pytest] command = "pytest -c pyproject.toml tests" # Extensions to
+pyproject.toml [tool.poetry.group.switchblade] optional = true
+[tool.poetry.group.switchblade.dependencies] pylint = "^2.17.2" pytest =
+"^7.3.1" [tool.pytest.ini_options] pythonpath = "src" ``` For each linter you
+want to add, specify a `[linters.]` section with a `command` key. The `command`
+value will be invoked by Switchblade when you run `swb lint `. The `[linters]`
+section specifies which linters should be invoked (and in which order) when you
+run `swb lint` or `swb lint all`. The same goes for tests: specify a `[tests.]`
+section with a `command` key, and add the tool to the `[tests]` section to have
+it invoked when you run `swb test` or `swb test all`. ### Tool configuration
+Anything in the `bundle.toml` file under a `tool.*` section will be temporarily
+added to the project's `pyproject.toml` file under that section. This allows
+you to add dependencies and configuration options to all your projects without
+having to manually edit all the individual `pyproject.toml` files. If you
+prefer having separate config files, or for tools which do not support
+`pyproject.toml` configuration, simply add any config files you need in the
+same folder as the `bundle.toml` file. E.g. you might define a `.pylintrc` in
+the bundle repo: ```ini [MAIN] [MESSAGES CONTROL] disable= C0111, # missing-
+docstring C0114, # missing-module-docstring C0115, # missing-class-docstring
+C0116, # missing-function-docstring W0613, # unused-argument ``` Now, when you
+want to use your custom dev tool bundle in a project, simply point to the repo
+in the project `.switchblade` file as in the example above. Swichblade will
+then fetch and install the tools you specified in the bundle and run them with
+the configurations you specified. ### Per-project overrides To override the
 bundle configuration for a specific dev tool in one of your project repos,
 simply check in the tool dependencies and configuration files in the project
 repo as you normally would - Switchblade will still invoke the dev tool, but it
 will not overwrite any existing config files or `[tool.*]` sections in your
-`pyproject.toml` file. Be aware that this does not \'extend\' the configuration
+`pyproject.toml` file. Be aware that this does not 'extend' the configuration
 from the bundle, but replaces that tool configuration entirely, so this feature
-should be used with caution.\n\nTo override the command or the list of linters
-to run, add the corresponding sections (e.g. `[linters]` or `[linters.pylint]`
-in the project `.switchblade` file. Switchblade will automatically merge (in
-this case it does extend rather than replace) the bundle config and Switchblade
-config before invoking any of the tools.\n\n## Prerequisites\n\n- [Python 3.7+]
-(https://www.python.org/downloads/)\n\nCurrently, you need Python since you
-install Switchblade with pip. This may change in the future.\n\n##
-Features\n\n- CLI command `swb lint` to run linters\n- CLI command `swb test`
-to run tests\n- Project \'modes\' supported: Currently only `python-poetry` is
-supported, but more will be added soon.\n\n## Development\n\nInstall
-dependencies:\n\n```shell\n> poetry install\n```\n\nRun unit tests with
-coverage:\n\n```shell\n> poetry run pytest -c pyproject.toml --cov-report=term
---cov=src tests\n```\n\nOr run unit tests on multiple Python versions with tox:
-\n\n```shell\n> poetry run tox\n```\n', 'author': 'JensRoland', 'author_email':
-'mail@jensroland.com', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
-'https://jensroland.com/sentient-switchblade', 'package_dir': package_dir,
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'entry_points': entry_points, 'python_requires':
-'>=3.7,<4.0', } setup(**setup_kwargs)
+should be used with caution. To override the command or the list of linters to
+run, add the corresponding sections (e.g. `[linters]` or `[linters.pylint]` in
+the project `.switchblade` file. Switchblade will automatically merge (in this
+case it does extend rather than replace) the bundle config and Switchblade
+config before invoking any of the tools. ## Prerequisites - [Python 3.7+]
+(https://www.python.org/downloads/) Currently, you need Python since you
+install Switchblade with pip. This may change in the future. ## Features - CLI
+command `swb lint` to run linters - CLI command `swb test` to run tests -
+Project 'modes' supported: Currently only `python-poetry` is supported, but
+more will be added soon. ## Development Install dependencies: ```shell > poetry
+install ``` Run unit tests with coverage: ```shell > poetry run pytest -
+c pyproject.toml --cov-report=term --cov=src tests ``` Or run unit tests on
+multiple Python versions with tox: ```shell > poetry run tox ```
```

