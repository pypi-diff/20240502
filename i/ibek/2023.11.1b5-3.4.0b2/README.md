# Comparing `tmp/ibek-2023.11.1b5.tar.gz` & `tmp/ibek-3.4.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibek-2023.11.1b5.tar", last modified: Fri Nov 10 10:40:16 2023, max compression
+gzip compressed data, was "ibek-3.4.0b2.tar", last modified: Mon Mar 25 12:55:57 2024, max compression
```

## Comparing `ibek-2023.11.1b5.tar` & `ibek-3.4.0b2.tar`

### file list

```diff
@@ -1,186 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.238645 ibek-2023.11.1b5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.218645 ibek-2023.11.1b5/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      537 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.devcontainer/local_build.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.218645 ibek-2023.11.1b5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.210645 ibek-2023.11.1b5/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.218645 ibek-2023.11.1b5/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.218645 ibek-2023.11.1b5/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     3041 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.218645 ibek-2023.11.1b5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (127)      598 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.218645 ibek-2023.11.1b5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      655 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20134 2023-11-10 10:40:16.238645 ibek-2023.11.1b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/builder2ibek.README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)    18331 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/builder2ibek.support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.218645 ibek-2023.11.1b5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.218645 ibek-2023.11.1b5/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.222645 ibek-2023.11.1b5/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.222645 ibek-2023.11.1b5/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (127)      558 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/developer/explanations/decisions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7669 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/developer/explanations/entities.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.222645 ibek-2023.11.1b5/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      820 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.222645 ibek-2023.11.1b5/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.222645 ibek-2023.11.1b5/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.222645 ibek-2023.11.1b5/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)     9460 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/images/ibek-arch.svg
--rw-r--r--   0 runner    (1001) docker     (127)    14318 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/images/ibek-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     9125 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/images/ibek-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.222645 ibek-2023.11.1b5/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.222645 ibek-2023.11.1b5/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.222645 ibek-2023.11.1b5/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/user/how-to/edit-yaml.rst
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.226645 ibek-2023.11.1b5/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/user/reference/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/user/reference/naming.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.226645 ibek-2023.11.1b5/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/docs/user/tutorials/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.226645 ibek-2023.11.1b5/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/examples/test_refs1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.226645 ibek-2023.11.1b5/examples/yaml/
--rwxr-xr-x   0 runner    (1001) docker     (127)      514 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/examples/yaml/test-ibek.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/examples/yaml/test.ibek.ioc.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/examples/yaml/test.ibek.ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/examples/yaml/test.ibek.support.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-10 10:40:16.238645 ibek-2023.11.1b5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.214645 ibek-2023.11.1b5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.226645 ibek-2023.11.1b5/src/ibek/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-11-10 10:40:16.000000 ibek-2023.11.1b5/src/ibek/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/gen_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/ioc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.230645 ibek-2023.11.1b5/src/ibek/ioc_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/ioc_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/ioc_cmds/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/ioc_cmds/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/ioc_cmds/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/render_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.230645 ibek-2023.11.1b5/src/ibek/runtime_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/runtime_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/runtime_cmds/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.230645 ibek-2023.11.1b5/src/ibek/support_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/support_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/support_cmds/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/support_cmds/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/support_cmds/files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.230645 ibek-2023.11.1b5/src/ibek/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.230645 ibek-2023.11.1b5/src/ibek/templates/ioc/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/ioc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.230645 ibek-2023.11.1b5/src/ibek/templates/ioc/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/ioc/config/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.230645 ibek-2023.11.1b5/src/ibek/templates/ioc/configure/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/ioc/configure/CONFIG
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/ioc/configure/CONFIG_SITE
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/ioc/configure/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/ioc/configure/RELEASE
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/ioc/configure/RULES
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/ioc/configure/RULES.ioc
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/ioc/configure/RULES_DIRS
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/ioc/configure/RULES_TOP
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.214645 ibek-2023.11.1b5/src/ibek/templates/ioc/iocApp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.234645 ibek-2023.11.1b5/src/ibek/templates/ioc/iocApp/src/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/ioc/iocApp/src/Makefile.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/ioc/iocApp/src/iocMain.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)     1050 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/ioc/liveness.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     4214 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/ioc/start.sh
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/ioc/stop.sh
--rw-r--r--   0 runner    (1001) docker     (127)      395 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/ioc.subst.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      366 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/st.cmd.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.234645 ibek-2023.11.1b5/src/ibek/templates/support/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/support/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.234645 ibek-2023.11.1b5/src/ibek/templates/support/configure/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/templates/support/configure/RELEASE
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/src/ibek/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.230645 ibek-2023.11.1b5/src/ibek.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20134 2023-11-10 10:40:16.000000 ibek-2023.11.1b5/src/ibek.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2023-11-10 10:40:16.000000 ibek-2023.11.1b5/src/ibek.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-10 10:40:16.000000 ibek-2023.11.1b5/src/ibek.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-10 10:40:16.000000 ibek-2023.11.1b5/src/ibek.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-11-10 10:40:16.000000 ibek-2023.11.1b5/src/ibek.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-10 10:40:16.000000 ibek-2023.11.1b5/src/ibek.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.234645 ibek-2023.11.1b5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1796 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/generate_samples.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.214645 ibek-2023.11.1b5/tests/samples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.214645 ibek-2023.11.1b5/tests/samples/epics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.234645 ibek-2023.11.1b5/tests/samples/epics/pvi-defs/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/epics/pvi-defs/simple.pvi.device.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.234645 ibek-2023.11.1b5/tests/samples/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/outputs/all.ioc.subst
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/outputs/all.st.cmd
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/outputs/index.bob
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/outputs/objects.ioc.subst
--rw-r--r--   0 runner    (1001) docker     (127)      828 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/outputs/objects.st.cmd
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/outputs/simple.pvi.bob
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/outputs/simple.pvi.template
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/outputs/utils.ioc.subst
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/outputs/utils.st.cmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.234645 ibek-2023.11.1b5/tests/samples/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    15525 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/schemas/ibek.support.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/schemas/multiple.ibek.ioc.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/schemas/objects.ibek.ioc.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/schemas/utils.ibek.ioc.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:40:16.238645 ibek-2023.11.1b5/tests/samples/yaml/
--rw-r--r--   0 runner    (1001) docker     (127)      874 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/yaml/all.ibek.ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/yaml/all.ibek.support.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/yaml/bad_counter.ibek.ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/yaml/bad_counter2.ibek.ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/yaml/bad_db.ibek.ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/yaml/bad_db.ibek.support.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/yaml/bad_default.ibek.ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/yaml/bad_ref.ibek.ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/yaml/objects.ibek.ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/yaml/objects.ibek.support.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/yaml/simple.pvi.device.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/yaml/utils.ibek.ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/samples/yaml/utils.ibek.support.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2894 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/sys-test.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2023-11-10 10:40:08.000000 ibek-2023.11.1b5/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.596970 ibek-3.4.0b2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.devcontainer/devcontainer.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.devcontainer/local_build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.568970 ibek-3.4.0b2/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3041 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-25 12:55:52.000000 ibek-3.4.0b2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-03-25 12:55:52.000000 ibek-3.4.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20089 2024-03-25 12:55:57.596970 ibek-3.4.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-03-25 12:55:52.000000 ibek-3.4.0b2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-25 12:55:52.000000 ibek-3.4.0b2/builder2ibek.README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19288 2024-03-25 12:55:52.000000 ibek-3.4.0b2/builder2ibek.support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/explanations/decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/explanations/entities.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/images/ibek-arch.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    14318 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/images/ibek-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/images/ibek-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/user/how-to/edit-yaml.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/user/reference/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/user/reference/naming.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/user/tutorials/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-25 12:55:52.000000 ibek-3.4.0b2/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-03-25 12:55:52.000000 ibek-3.4.0b2/examples/test_refs1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.584970 ibek-3.4.0b2/examples/yaml/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      514 2024-03-25 12:55:52.000000 ibek-3.4.0b2/examples/yaml/test-ibek.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-25 12:55:52.000000 ibek-3.4.0b2/examples/yaml/test.ibek.ioc.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-25 12:55:52.000000 ibek-3.4.0b2/examples/yaml/test.ibek.ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-25 12:55:52.000000 ibek-3.4.0b2/examples/yaml/test.ibek.support.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-03-25 12:55:52.000000 ibek-3.4.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 12:55:57.596970 ibek-3.4.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.572970 ibek-3.4.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.584970 ibek-3.4.0b2/src/ibek/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-25 12:55:57.000000 ibek-3.4.0b2/src/ibek/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.584970 ibek-3.4.0b2/src/ibek/dev_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/dev_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/dev_cmds/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/gen_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/ioc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.588970 ibek-3.4.0b2/src/ibek/ioc_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/ioc_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/ioc_cmds/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/ioc_cmds/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/ioc_cmds/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/render_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.588970 ibek-3.4.0b2/src/ibek/runtime_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/runtime_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/runtime_cmds/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.588970 ibek-3.4.0b2/src/ibek/support_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/support_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/support_cmds/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/support_cmds/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/support_cmds/files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.588970 ibek-3.4.0b2/src/ibek/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/templates/ioc.subst.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/templates/st.cmd.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.588970 ibek-3.4.0b2/src/ibek/templates/support/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/templates/support/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.588970 ibek-3.4.0b2/src/ibek/templates/support/configure/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/templates/support/configure/RELEASE
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.596970 ibek-3.4.0b2/src/ibek.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20089 2024-03-25 12:55:57.000000 ibek-3.4.0b2/src/ibek.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-03-25 12:55:57.000000 ibek-3.4.0b2/src/ibek.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 12:55:57.000000 ibek-3.4.0b2/src/ibek.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-25 12:55:57.000000 ibek-3.4.0b2/src/ibek.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-25 12:55:57.000000 ibek-3.4.0b2/src/ibek.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-25 12:55:57.000000 ibek-3.4.0b2/src/ibek.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.588970 ibek-3.4.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1760 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/generate_samples.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.572970 ibek-3.4.0b2/tests/samples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.572970 ibek-3.4.0b2/tests/samples/epics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.592970 ibek-3.4.0b2/tests/samples/epics/pvi-defs/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/epics/pvi-defs/simple.pvi.device.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.592970 ibek-3.4.0b2/tests/samples/iocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/iocs/bad_counter.ibek.ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/iocs/bad_counter2.ibek.ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/iocs/bad_db.ibek.ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/iocs/bad_default.ibek.ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/iocs/bad_ref.ibek.ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/iocs/ibek-mo-ioc-01.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/iocs/utils.ibek.ioc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.572970 ibek-3.4.0b2/tests/samples/outputs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.592970 ibek-3.4.0b2/tests/samples/outputs/motorSim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/outputs/motorSim/index.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/outputs/motorSim/ioc.subst
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/outputs/motorSim/simple.pvi.bob
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/outputs/motorSim/simple.pvi.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/outputs/motorSim/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.592970 ibek-3.4.0b2/tests/samples/outputs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/outputs/utils/index.bob
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/outputs/utils/ioc.subst
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/outputs/utils/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.592970 ibek-3.4.0b2/tests/samples/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/schemas/ibek.support.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/schemas/motorSim.ibek.ioc.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/schemas/single.ibek.ioc.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/schemas/utils.ibek.ioc.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.596970 ibek-3.4.0b2/tests/samples/support/
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/support/asyn.ibek.support.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/support/bad_db.ibek.support.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/support/motorSim.ibek.support.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/support/simple.pvi.device.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/support/utils.ibek.support.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2894 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/sys-test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/test_unit.py
```

### Comparing `ibek-2023.11.1b5/.devcontainer/devcontainer.json` & `ibek-3.4.0b2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/.devcontainer/local_build.sh` & `ibek-3.4.0b2/.devcontainer/local_build.sh`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/.github/CONTRIBUTING.rst` & `ibek-3.4.0b2/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/.github/actions/install_requirements/action.yml` & `ibek-3.4.0b2/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/.github/dependabot.yml` & `ibek-3.4.0b2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/.github/pages/make_switcher.py` & `ibek-3.4.0b2/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/.github/workflows/code.yml` & `ibek-3.4.0b2/.github/workflows/code.yml`

 * *Files 10% similar despite different names*

```diff
@@ -65,15 +65,15 @@
       - name: List dependency tree
         run: pipdeptree
 
       - name: Run tests
         run: tox -e pytest
 
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with:
           name: ${{ matrix.python }}/${{ matrix.os }}
           files: cov.xml
 
   dist:
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     runs-on: "ubuntu-latest"
@@ -111,42 +111,43 @@
         run: python -m $(ls src | head -1) --version
 
   release:
     # upload to PyPI and make a release on every tag
     needs: [lint, dist, test]
     if: ${{ github.event_name == 'push' && github.ref_type == 'tag' }}
     runs-on: ubuntu-latest
-    env:
-      HAS_PYPI_TOKEN: ${{ secrets.PYPI_TOKEN != '' }}
+    permissions:
+      # this permission is mandatory for trusted publishing To PyPI
+      id-token: write
+      contents: write
+    # Specify the GitHub Environment to publish to
+    environment: release
 
     steps:
       - name: Checkout
         uses: actions/checkout@v4
 
       - uses: actions/download-artifact@v3
 
       - name: Fixup blank lockfiles
         # Github release artifacts can't be blank
         run: for f in lockfiles/*; do [ -s $f ] || echo '# No requirements' >> $f; done
 
       - name: Github Release
         # We pin to the SHA, not the tag, for security reasons.
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
-        uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844 # v0.1.15
+        uses: softprops/action-gh-release@9d7c94cfd0a1f3ed45544c887983e9fa900f0564 # v0.1.15
         with:
           prerelease: ${{ contains(github.ref_name, 'a') || contains(github.ref_name, 'b') || contains(github.ref_name, 'rc') }}
           # upload distribution files and lockfiles plus the support YAML schema
           # note that the 'sample' has been checked to be current by the tests
           files: |
             dist/*
             lockfiles/*
             tests/samples/schemas/ibek.support.schema.json
           generate_release_notes: true
 
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Publish to PyPI
-        if: ${{ env.HAS_PYPI_TOKEN }}
         uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `ibek-2023.11.1b5/.github/workflows/docs.yml` & `ibek-3.4.0b2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/.github/workflows/docs_clean.yml` & `ibek-3.4.0b2/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/.gitignore` & `ibek-3.4.0b2/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -73,10 +73,9 @@
 # default filename for builder2ibek
 **/ibek.support.yaml
 # this file may be created accidentally by ibek being run in its own directory
 # so we ignore it
 config/
 
 # generated test files
-tests/samples/epics/opi
 tests/samples/epics/runtime
-
+tests/samples/epics/opi
```

### Comparing `ibek-2023.11.1b5/.vscode/launch.json` & `ibek-3.4.0b2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/LICENSE` & `ibek-3.4.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/PKG-INFO` & `ibek-3.4.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibek
-Version: 2023.11.1b5
+Version: 3.4.0b2
 Summary: IOC Builder for EPICS and Kubernetes
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,30 +209,29 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: pydantic==2.3.0
+Requires-Dist: pydantic==2.6.4
 Requires-Dist: typer
 Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2
 Requires-Dist: GitPython
-Requires-Dist: pvi>=0.6
+Requires-Dist: pvi~=0.8
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pipdeptree; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pydata-sphinx-theme>=0.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
-Requires-Dist: pytest-env; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: Sphinx==6.2.1; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinx-design; extra == "dev"
 Requires-Dist: tox-direct; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
@@ -244,14 +243,15 @@
 
 
 This tool supports building container images for Generic EPICS IOCs and
 generating IOC Instances from those Generic IOCs at container runtime. It is
 targetted at running IOCs in Kubernetes, but the images it
 creates can execute in any container runtime, such as docker or podman.
 
+
   ============== ==============================================================
   PyPI           ``pip install ibek``
   Source code    https://github.com/epics-containers/ibek
   Documentation  https://epics-containers.github.io/ibek
   Releases       https://github.com/epics-containers/ibek/releases
   ============== ==============================================================
```

### Comparing `ibek-2023.11.1b5/README.rst` & `ibek-3.4.0b2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 This tool supports building container images for Generic EPICS IOCs and
 generating IOC Instances from those Generic IOCs at container runtime. It is
 targetted at running IOCs in Kubernetes, but the images it
 creates can execute in any container runtime, such as docker or podman.
 
+
   ============== ==============================================================
   PyPI           ``pip install ibek``
   Source code    https://github.com/epics-containers/ibek
   Documentation  https://epics-containers.github.io/ibek
   Releases       https://github.com/epics-containers/ibek/releases
   ============== ==============================================================
```

### Comparing `ibek-2023.11.1b5/builder2ibek.README.md` & `ibek-3.4.0b2/builder2ibek.README.md`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/builder2ibek.support.py` & `ibek-3.4.0b2/builder2ibek.support.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,20 +137,33 @@
                 description_str = "TODO: ADD DESCRIPTION"
 
             if arg_name not in self.all_args:
                 new_yaml_arg = ordereddict()
                 new_yaml_arg["type"] = typ
                 new_yaml_arg["name"] = arg_name
                 new_yaml_arg["description"] = PreservedScalarString(description_str)
-                if default:
+                if default is not None:
                     new_yaml_arg["default"] = default
                 if typ == "enum":
                     new_yaml_arg["values"] = {
                         str(label): None for label in details.labels
                     }
+                # coerce type of args that have default strings which are ints or reals
+                if typ == "str" and default:
+                    try:
+                        i = int(default)
+                        new_yaml_arg["default"] = i
+                        new_yaml_arg["type"] = "int"
+                    except ValueError:
+                        try:
+                            f = float(default)
+                            new_yaml_arg["default"] = f
+                            new_yaml_arg["type"] = "float"
+                        except ValueError:
+                            pass
 
                 self.yaml_args.append(new_yaml_arg)
                 self.all_args.append(arg_name)
 
     def make_arg(self, name, details, default=None):
         """
         Work out the type and default value for an argument.
@@ -194,14 +207,15 @@
         if name == "CS":
             typ = "int"
             value = MagicMock()
 
         if name not in self.builder_args:
             if ArgInfo.arg_num in self.overrides:
                 value = self.overrides[ArgInfo.arg_num]
+                typ = type(value).__name__
 
             self.builder_args[name] = value
 
             if isinstance(value, MagicMock):
                 value = "Object" + str(ArgInfo.arg_num)
             print(
                 "    ARG {:3} {:20} {:<20} {}".format(ArgInfo.arg_num, name, value, typ)
@@ -363,14 +377,16 @@
                     line = macros_re.sub(macro_to_jinja_re, matches[0][1])
                     commands += line + "\n"
             if commands:
                 script_text = PreservedScalarString(commands)
                 missing = set(command_args) - set(arginfo.all_args)
                 comment = MISSING + ", ".join(missing) if missing else None
 
+                # remove spurious \n from the script text (not newlines)
+                script_text = script_text.replace(r"\n", "")
                 script_item.insert(3, "value", script_text, comment=comment)
 
             script.append(script_item)
 
     def parse_initialise_functions(self, builder_object, arginfo):
         """
         Extract the code from the builder class Initialise() method
@@ -420,38 +436,41 @@
         """
         Convert the yaml object graph into a YAML file
         """
 
         def tidy_up(yaml):
             # add blank lines between major fields
             for field in [
-                "- name:",
-                "  databases:",
-                "  pre_init:",
-                "  post_init:",
+                "  - name:",
+                "    databases:",
+                "    pre_init:",
+                "    post_init:",
                 "module",
                 "defs",
-                "  - type:",
+                "      - type:",
+                "      - file:",
+                "      - value:",
             ]:
                 yaml = re.sub(r"(\n%s)" % field, "\n\\g<1>", yaml)
-
             return yaml
 
         yaml = YAML()
 
         yaml.default_flow_style = False
 
         # add support yaml schema
         self.yaml_tree.yaml_add_eol_comment(
             "yaml-language-server: $schema=https://github.com/epics-"
-            "containers/ibek/releases/download/1.2.0/ibek.support.schema.json"
+            "containers/ibek/releases/download/1.2.0/ibek.support.schema.json",
+            column=0,
         )
 
         print("\nWriting YAML output to %s ..." % filename)
         with open(filename, "wb") as f:
+            yaml.indent(mapping=2, sequence=4, offset=2)
             yaml.dump(self.yaml_tree, f, transform=tidy_up)
 
 
 def parse_args():
     """
     Parse the command line arguments
     """
```

### Comparing `ibek-2023.11.1b5/docs/conf.py` & `ibek-3.4.0b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst` & `ibek-3.4.0b2/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/developer/explanations/decisions.rst` & `ibek-3.4.0b2/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/developer/explanations/entities.rst` & `ibek-3.4.0b2/docs/developer/explanations/entities.rst`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 Expand below for the example **support module definition file**:
 
     .. raw:: html
 
         <details>
         <summary><a>objects.ibek.support.yaml</a></summary>
 
-    .. include:: ../../../tests/samples/yaml/objects.ibek.support.yaml
+    .. include:: ../../../tests/samples/support/motorSim.ibek.support.yaml
         :literal:
 
     .. raw:: html
 
         </details>
 
 Definition is implemented in the code using a class of the same name.
@@ -145,24 +145,24 @@
 Click the arrows to reveal the files.
 
     .. raw:: html
 
         <details>
         <summary><a>all.ibek.ioc.yaml</a></summary>
 
-    .. include:: ../../../tests/samples/yaml/all.ibek.ioc.yaml
+    .. include:: ../../../tests/samples/iocs/ibek-mo-ioc-01.yaml
         :literal:
 
     .. raw:: html
 
         </details>
         <details>
         <summary><a>st.cmd</a></summary>
 
-    .. include:: ../../../tests/samples/outputs/all.st.cmd
+    .. include:: ../../../tests/samples/outputs/motorSim/st.cmd
         :literal:
 
     .. raw:: html
 
         </details>
 
 Entity is implemented in the code using a class of the same name.
@@ -216,15 +216,15 @@
 
     .. raw:: html
 
         </details>
         <details>
         <summary><a>multiple.ibek.ioc.schema.json</a></summary>
 
-    .. include:: ../../../tests/samples/schemas/multiple.ibek.ioc.schema.json
+    .. include:: ../../../tests/samples/schemas/single.ibek.ioc.schema.json
         :literal:
 
     .. raw:: html
 
         </details>
 
 This results in the overall generated file structure:
```

### Comparing `ibek-2023.11.1b5/docs/developer/how-to/build-docs.rst` & `ibek-3.4.0b2/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/developer/how-to/lint.rst` & `ibek-3.4.0b2/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/developer/how-to/make-release.rst` & `ibek-3.4.0b2/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/developer/how-to/pin-requirements.rst` & `ibek-3.4.0b2/docs/developer/how-to/pin-requirements.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/developer/how-to/test-container.rst` & `ibek-3.4.0b2/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/developer/how-to/update-tools.rst` & `ibek-3.4.0b2/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/developer/index.rst` & `ibek-3.4.0b2/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/developer/reference/standards.rst` & `ibek-3.4.0b2/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/developer/tutorials/dev-install.rst` & `ibek-3.4.0b2/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/images/ibek-arch.svg` & `ibek-3.4.0b2/docs/images/ibek-arch.svg`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/images/ibek-favicon.ico` & `ibek-3.4.0b2/docs/images/ibek-favicon.ico`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/images/ibek-logo.svg` & `ibek-3.4.0b2/docs/images/ibek-logo.svg`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/index.rst` & `ibek-3.4.0b2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/user/explanations/docs-structure.rst` & `ibek-3.4.0b2/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/user/index.rst` & `ibek-3.4.0b2/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/user/reference/api.rst` & `ibek-3.4.0b2/docs/user/reference/api.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/user/reference/naming.rst` & `ibek-3.4.0b2/docs/user/reference/naming.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/docs/user/tutorials/installation.rst` & `ibek-3.4.0b2/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/examples/README.md` & `ibek-3.4.0b2/examples/README.md`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/examples/test_refs1.py` & `ibek-3.4.0b2/examples/test_refs1.py`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/examples/yaml/test-ibek.sh` & `ibek-3.4.0b2/examples/yaml/test-ibek.sh`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/examples/yaml/test.ibek.ioc.schema.json` & `ibek-3.4.0b2/examples/yaml/test.ibek.ioc.schema.json`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/examples/yaml/test.ibek.support.yaml` & `ibek-3.4.0b2/examples/yaml/test.ibek.support.yaml`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/pyproject.toml` & `ibek-3.4.0b2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 description = "IOC Builder for EPICS and Kubernetes"
 dependencies = [
-    "pydantic==2.3.0",
+    "pydantic==2.6.4",
     "typer",
     "ruamel.yaml",
     "jinja2",
     "GitPython",
-    "pvi>=0.6",
+    "pvi~=0.8",  # pvi currently tracks breaking changes with minor version
 ] # Add project dependencies here, e.g. ["click", "numpy"]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.rst"
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
@@ -30,15 +30,14 @@
     "mypy",
     "pipdeptree",
     "pre-commit",
     "pydata-sphinx-theme>=0.12",
     "pytest",
     "pytest-cov",
     "pytest-mock",
-    "pytest-env",
     "ruff",
     "Sphinx==6.2.1",
     "sphinx-autobuild",
     "sphinx-copybutton",
     "sphinx-design",
     "tox-direct",
     "types-mock",
@@ -64,15 +63,19 @@
 [tool.pytest.ini_options]
 # Run pytest with all our checkers, and don't spam us with massive tracebacks on error
 addopts = """
     --tb=native -vv --doctest-modules --doctest-glob="*.rst"
     --cov=ibek --cov-report term --cov-report xml:cov.xml
     """
 # https://iscinumpy.gitlab.io/post/bound-version-constraints/#watch-for-warnings
-filterwarnings = ["error", "ignore::pytest_cov.plugin.CovDisabledWarning"]
+filterwarnings = [
+    "error",
+    "ignore::pytest_cov.plugin.CovDisabledWarning",
+    "ignore:'autocompletion' is renamed to 'shell_complete'. The old name is deprecated and will be removed in Click 8.1. See the docs about 'Parameter' for information about new behavior.:DeprecationWarning:typer",
+]
 # Doctest python code in docs, python code in src docstrings, test functions in tests
 testpaths = "docs src tests"
 
 [tool.coverage.run]
 data_file = "/tmp/ibek.coverage"
 
 [tool.coverage.paths]
@@ -99,14 +102,15 @@
 commands =
     pytest: pytest --cov=ibek --cov-report term --cov-report xml:cov.xml {posargs}
     mypy: mypy src tests {posargs}
     pre-commit: pre-commit run --all-files {posargs}
     docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html
 """
 
+
 [tool.ruff]
 src = ["src", "tests"]
 ignore = [
     "C408", # Unnecessary collection call - e.g. list(...) instead of [...]
     "E501", # Line too long, should be fixed by black.
 ]
 line-length = 88
```

### Comparing `ibek-2023.11.1b5/src/ibek/__main__.py` & `ibek-3.4.0b2/src/ibek/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
 
 import typer
 from ruamel.yaml import YAML
 
 from ibek._version import __version__
+from ibek.dev_cmds.commands import dev_cli
 from ibek.globals import NaturalOrderGroup
 from ibek.ioc_cmds.commands import ioc_cli
 from ibek.runtime_cmds.commands import runtime_cli
 from ibek.support_cmds.commands import support_cli
 
 cli = typer.Typer(cls=NaturalOrderGroup)
 
@@ -22,14 +23,19 @@
     help="Commands for building generic IOCs during container build",
 )
 cli.add_typer(
     runtime_cli,
     name="runtime",
     help="Commands for building IOC instance startup files at container runtime",
 )
+cli.add_typer(
+    dev_cli,
+    name="dev",
+    help="Commands for working inside Generic IOC development containers",
+)
 
 yaml = YAML()
 
 
 def version_callback(value: bool):
     if value:
         typer.echo(__version__)
```

### Comparing `ibek-2023.11.1b5/src/ibek/gen_scripts.py` & `ibek-3.4.0b2/src/ibek/gen_scripts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Functions for building the db and boot scripts
 """
+
 import logging
 import re
 from pathlib import Path
 from typing import List, Tuple, Type
 
 from jinja2 import Template
 from ruamel.yaml.main import YAML
 
+from ibek.utils import UTILS
+
 from .globals import TEMPLATES
 from .ioc import IOC, Entity, clear_entity_model_ids, make_entity_models, make_ioc_model
 from .render import Render
 from .render_db import RenderDb
 from .support import Database, Support
 
 log = logging.getLogger(__name__)
@@ -51,14 +54,23 @@
 
     Returns a model of the resulting ioc instance
     """
     ioc_model = ioc_create_model(definition_yaml)
 
     # extract the ioc instance yaml into a dict
     ioc_instance_dict = YAML(typ="safe").load(ioc_instance_yaml)
+    if ioc_instance_dict is None or "ioc_name" not in ioc_instance_dict:
+        raise RuntimeError(
+            f"Failed to load a valid ioc config from {ioc_instance_yaml}"
+        )
+
+    # extract the ioc name into UTILS for use in jinja renders
+    name = UTILS.render({}, ioc_instance_dict["ioc_name"])
+    UTILS.set_ioc_name(name)
+    ioc_instance_dict["ioc_name"] = name
 
     # Create an IOC instance from the instance dict and the model
     ioc_instance = ioc_model(**ioc_instance_dict)
 
     return ioc_instance
 
 
@@ -84,11 +96,12 @@
     """
     with open(TEMPLATES / "st.cmd.jinja", "r") as f:
         template = Template(f.read())
 
     renderer = Render()
 
     return template.render(
+        __utils__=UTILS,
         env_var_elements=renderer.render_environment_variable_elements(ioc_instance),
         script_elements=renderer.render_pre_ioc_init_elements(ioc_instance),
         post_ioc_init_elements=renderer.render_post_ioc_init_elements(ioc_instance),
     )
```

### Comparing `ibek-2023.11.1b5/src/ibek/ioc.py` & `ibek-3.4.0b2/src/ibek/ioc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Functions for generating an IocInstance derived class from a
 support module definition YAML file
 """
+
 from __future__ import annotations
 
 import builtins
 from enum import Enum
 from typing import Annotated, Any, Dict, Literal, Sequence, Tuple, Type, Union
 
 from pydantic import (
@@ -13,16 +14,17 @@
     create_model,
     field_validator,
     model_validator,
 )
 from pydantic.fields import FieldInfo
 from pydantic_core import PydanticUndefined
 
-from .globals import BaseSettings, render_with_utils
+from .globals import BaseSettings
 from .support import Definition, EnumArg, IdArg, ObjectArg, Support
+from .utils import UTILS
 
 id_to_entity: Dict[str, Entity] = {}
 
 
 class EnumVal(Enum):
     """
     An enum that is printed as its name only
@@ -57,15 +59,15 @@
             if arg in ids:
                 # add this entity to the global id index
                 if value in id_to_entity:
                     raise ValueError(f"Duplicate id {value} in {list(id_to_entity)}")
                 id_to_entity[value] = entity
             elif isinstance(value, str):
                 # Jinja expansion of any of the Entity's string args/values
-                setattr(entity, arg, render_with_utils(entity_dict, value))
+                setattr(entity, arg, UTILS.render(entity_dict, value))
         return entity
 
     def __str__(self):
         # if this entity has an id then its string representation is the value of id
         id_name = self.__definition__._get_id_arg()
         return getattr(self, id_name) if id_name else super().__str__()
```

### Comparing `ibek-2023.11.1b5/src/ibek/ioc_cmds/assets.py` & `ibek-3.4.0b2/src/ibek/ioc_cmds/assets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,19 @@
+import logging
 import os
 import shutil
 import subprocess
 from pathlib import Path
 from typing import List
 
 import typer
 
-from ibek.globals import EPICS_ROOT, IBEK_DEFS, IOC_FOLDER, PVI_DEFS
+from ibek.globals import GLOBALS, IOC_FOLDER
 
-
-def get_ioc_source() -> Path:
-    """
-    The generic ioc source folder is mounted into the container at
-    /epics/ioc-XXXXX and should always contain the ibek-support
-    submodule. Therefore we can find the ibek-support folder by looking
-    for the ibek-support folder.
-
-    Functions that use this should provide an override variable that allows
-    the ibek caller to specify the location.
-    """
-    try:
-        ibek_support = (
-            list(EPICS_ROOT.glob("*/ibek-support"))
-            or list(Path("..").glob("/**/ibek-support"))
-        )[0]
-    except IndexError:
-        raise RuntimeError(
-            "Could NOT find a suitable location for the IOC source folder. "
-            "ibek must be run in a container with the generic IOC source folder"
-        )
-    return (ibek_support / "..").resolve()
+log = logging.getLogger(__name__)
 
 
 def move_file(src: Path, dest: Path, binary: List[str]):
     """
     Move a file / tree / symlink from src to dest, stripping symbols from
     binaries if they are in the binary list.
     """
@@ -51,39 +31,68 @@
             raise RuntimeError(f"Failed to move {src} to {dest}")
     if dest.name in binary:
         # strip the symbols from the binary
         cmd = f"strip $(find {dest} -type f) &> /dev/null"
         subprocess.call(["bash", "-c", cmd])
 
 
-def extract_assets(destination: Path, source: Path, extras: List[Path], defaults: bool):
+def extract_assets(
+    destination: Path,
+    source: Path,
+    extras: List[Path],
+    defaults: bool,
+    dry_run: bool = False,
+):
     """
     extract and copy runtime assets from a completed developer stage container
     """
-    asset_matches = "bin|configure|db|dbd|include|lib|template|config|*.sh"
+
+    if GLOBALS.STATIC_BUILD:
+        # static builds only need database files from support modules
+        asset_matches = "db"
+    else:
+        # dynamically linked builds need binaries
+        asset_matches = "bin|db|lib"
 
     # chdir out of the folders we will move
     os.chdir(source)
 
     # a default set of assets that all IOCs will need at runtime
     if defaults:
         default_assets = [
-            get_ioc_source() / "ibek-support",
             source / "support" / "configure",
-            PVI_DEFS,
-            IBEK_DEFS,
-            IOC_FOLDER,
-            Path("/venv"),
-        ]
+            GLOBALS.PVI_DEFS,
+            GLOBALS.IBEK_DEFS,
+            IOC_FOLDER,  # get the IOC folder symlink
+            Path.readlink(IOC_FOLDER),  # get contents of IOC folder
+            Path("/venv"),  # get the virtualenv
+        ] + list(
+            source.glob("ibek*")
+        )  # get ibek-support and related folders
     else:
         default_assets = []
 
-    # identify EPICS modules as folders with binary output folders
+    # folder names with binary files in them
     binary = ["bin", "lib"]
 
+    # move the default assets and extras in their entirety
+    extra_files = default_assets + extras
+    for asset in extra_files:
+        src = source / asset
+        if src.exists():
+            dest_file = destination / asset.relative_to("/")
+            if dry_run:
+                typer.echo(f"Would move extra asset {src} to {dest_file} with {binary}")
+            else:
+                move_file(src, dest_file, binary)
+        else:
+            typer.echo(f"WARNING: runtime asset {src} missing")
+
+    # identify EPICS modules as folders with binary output folders
+    # and move only their output folders as specified by asset_matches
     binaries: List[Path] = []
     for find in binary:
         # only look two levels deep
         binaries.extend(source.glob(f"*/*/{find}"))
         binaries.extend(source.glob(f"*/{find}"))
 
     modules = [binary.parent for binary in binaries]
@@ -99,17 +108,11 @@
             asset for asset_glob in asset_globs for asset in asset_glob
         ]
 
         for asset in assets:
             src = module / asset
             if src.exists():
                 dest_file = destination_module / asset.relative_to(module)
-                move_file(src, dest_file, binary)
-
-    extra_files = default_assets + extras
-    for asset in extra_files:
-        src = source / asset
-        if src.exists():
-            dest_file = destination / asset.relative_to("/")
-            move_file(src, dest_file, binary)
-        else:
-            raise RuntimeError(f"extra runtime asset {src} missing")
+                if dry_run:
+                    typer.echo(f"Would move {src} to {dest_file} with {binary}")
+                else:
+                    move_file(src, dest_file, binary)
```

### Comparing `ibek-2023.11.1b5/src/ibek/ioc_cmds/docker.py` & `ibek-3.4.0b2/src/ibek/ioc_cmds/docker.py`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/src/ibek/render.py` & `ibek-3.4.0b2/src/ibek/render.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Functions for rendering lines in the boot script using Jinja2
 """
 
 from typing import Callable, List, Optional, Union
 
-from .globals import render_with_utils
 from .ioc import IOC, Entity
 from .support import Comment, Script, Text, When
+from .utils import UTILS
 
 
 class Render:
     """
     A class for generating snippets of startup script / EPICS DB
     by using Jinja to combine snippet templates from support module
     definition yaml with substitution values supplied in ioc entity yaml
@@ -41,15 +41,15 @@
                 self.once_done.append(name)
             else:
                 return ""
         elif when == When.last.value:
             raise NotImplementedError("When.last not yet implemented")
 
         # Render Jinja entries in the text
-        result = render_with_utils(instance, text)  # type: ignore
+        result = UTILS.render(instance, text)  # type: ignore
 
         if result == "":
             return ""
 
         return result + "\n"
 
     def render_script(self, instance: Entity, script_items: Script) -> Optional[str]:
@@ -93,15 +93,18 @@
         if not variables:
             return None
 
         env_var_txt = ""
         for variable in variables:
             # Substitute the name and value of the environment variable from args
             env_template = f"epicsEnvSet {variable.name} {variable.value}"
-            env_var_txt += render_with_utils(instance, env_template)  # type: ignore
+            env_var_txt += UTILS.render(
+                instance,
+                env_template,
+            )  # type: ignore
         return env_var_txt + "\n"
 
     def render_elements(
         self, ioc: IOC, method: Callable[[Entity], Union[str, None]]
     ) -> str:
         """
         Render elements of a given IOC instance based on calling the correct method
```

### Comparing `ibek-2023.11.1b5/src/ibek/render_db.py` & `ibek-3.4.0b2/src/ibek/render_db.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 A class for rendering a substitution file from multiple instantiations of
 support module definitions
 """
 
 from dataclasses import dataclass
 from typing import Any, Dict, List, Mapping, Optional, Tuple
 
-from ibek.globals import render_with_utils
 from ibek.ioc import IOC, Entity
 from ibek.support import Database
+from ibek.utils import UTILS
+
+
+def str_to_bool(v):
+    return v.lower() in ("yes", "true", "1")
 
 
 class RenderDb:
     @dataclass
     class RenderDbTemplate:
         filename: str
         rows: List[List[str]]
@@ -25,33 +29,27 @@
 
     def add_row(self, filename: str, args: Mapping[str, Any], entity: Entity) -> None:
         """
         Accumulate rows of arguments for each template file,
         Adding a new template file if it does not already exist.
         Convert all arguments to strings.
         """
-        filename = render_with_utils(dict(entity), filename)
+        filename = UTILS.render(dict(entity), filename)
 
         if filename not in self.render_templates:
             # for new filenames create a new RenderDbTemplate entry
             headings = [str(i) for i in list(args.keys())]
             self.render_templates[filename] = RenderDb.RenderDbTemplate(
                 filename=filename,
                 rows=[headings],  # first row is the headings
                 columns=[0] * len(args),
             )
 
-        # Add a new row of argument values.
-        # Note the case where no value was specified for the argument
-        # meaning that the name is to be rendered in Jinja
-        row = ["{{ %s }}" % k if v is None else v for k, v in args.items()]
-
-        # render any Jinja fields in the arguments
-        for i, line in enumerate(row):
-            row[i] = render_with_utils(dict(entity), row[i])
+        # add a new row of argument values, rendering any Jinja template fields
+        row = list(UTILS.render_map(dict(entity), args).values())
 
         # save the new row
         self.render_templates[filename].rows.append(row)
 
     def parse_instances(self) -> None:
         """
         Gather the database template instantiations from all entities
@@ -69,25 +67,26 @@
         """Validate database and add row using entity as context.
 
         Args:
             database: Database to add row for
             entity: Entity to use as context for Jinja template expansion
 
         """
-        database.file = database.file.strip("\n")
+        if str_to_bool(UTILS.render(entity, database.enabled)):
+            database.file = database.file.strip("\n")
 
-        for arg, value in database.args.items():
-            if value is None:
-                if arg not in entity.__dict__:
-                    raise ValueError(
-                        f"database arg '{arg}' in database template "
-                        f"'{database.file}' not found in context"
-                    )
+            for arg, value in database.args.items():
+                if value is None:
+                    if arg not in entity.__dict__:
+                        raise ValueError(
+                            f"database arg '{arg}' in database template "
+                            f"'{database.file}' not found in context"
+                        )
 
-        self.add_row(database.file, database.args, entity)
+            self.add_row(database.file, database.args, entity)
 
     def add_extra_databases(self, databases: List[Tuple[Database, Entity]]) -> None:
         """Add databases that are not part of Entity definitions
 
         Args:
             databases: Databases to add, each mapped against an Entity to use as context
```

### Comparing `ibek-2023.11.1b5/src/ibek/runtime_cmds/commands.py` & `ibek-3.4.0b2/src/ibek/runtime_cmds/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,70 +5,61 @@
 import typer
 from pvi._format.base import IndexEntry
 from pvi._format.dls import DLSFormatter
 from pvi._format.template import format_template
 from pvi.device import Device
 
 from ibek.gen_scripts import create_boot_script, create_db_script, ioc_deserialize
-from ibek.globals import (
-    OPI_OUTPUT_PATH,
-    PVI_DEFS,
-    RUNTIME_OUTPUT_PATH,
-    NaturalOrderGroup,
-    render_with_utils,
-)
+from ibek.globals import GLOBALS, NaturalOrderGroup
 from ibek.ioc import IOC, Entity
 from ibek.support import Database
+from ibek.utils import UTILS
 
 runtime_cli = typer.Typer(cls=NaturalOrderGroup)
 
-PVI_PV_PREFIX = "${prefix}"
-
 
 @runtime_cli.command()
 def generate(
     instance: Path = typer.Argument(
-        ..., help="The filepath to the ioc instance entity file"
+        ...,
+        help="The filepath to the ioc instance entity file",
+        autocompletion=lambda: [],  # Forces path autocompletion
     ),
     definitions: List[Path] = typer.Argument(
-        ..., help="The filepath to a support module definition file"
-    ),
-    out: Path = typer.Option(
-        default=RUNTIME_OUTPUT_PATH / "st.cmd",
-        help="Path to output startup script",
-    ),
-    db_out: Path = typer.Option(
-        default=RUNTIME_OUTPUT_PATH / "ioc.subst",
-        help="Path to output database expansion shell script",
+        ...,
+        help="The filepath to a support module definition file",
+        autocompletion=lambda: [],  # Forces path autocompletion
     ),
 ):
     """
     Build a startup script for an IOC instance
     """
+    # the file name under of the instance definition provides the IOC name
+    UTILS.set_file_name(instance)
+
     ioc_instance = ioc_deserialize(instance, definitions)
 
-    # Clear out generated files so developers know if something stop being generated
-    shutil.rmtree(RUNTIME_OUTPUT_PATH, ignore_errors=True)
-    RUNTIME_OUTPUT_PATH.mkdir(exist_ok=True)
-    shutil.rmtree(OPI_OUTPUT_PATH, ignore_errors=True)
-    OPI_OUTPUT_PATH.mkdir(exist_ok=True)
+    # Clear out generated files so developers know if something stops being generated
+    shutil.rmtree(GLOBALS.RUNTIME_OUTPUT, ignore_errors=True)
+    GLOBALS.RUNTIME_OUTPUT.mkdir(exist_ok=True)
+    shutil.rmtree(GLOBALS.OPI_OUTPUT, ignore_errors=True)
+    GLOBALS.OPI_OUTPUT.mkdir(exist_ok=True)
 
     pvi_index_entries, pvi_databases = generate_pvi(ioc_instance)
     generate_index(ioc_instance.ioc_name, pvi_index_entries)
 
     script_txt = create_boot_script(ioc_instance)
-
-    out.parent.mkdir(parents=True, exist_ok=True)
-
-    with out.open("w") as stream:
+    script_output = GLOBALS.RUNTIME_OUTPUT / "st.cmd"
+    script_output.parent.mkdir(parents=True, exist_ok=True)
+    with script_output.open("w") as stream:
         stream.write(script_txt)
 
     db_txt = create_db_script(ioc_instance, pvi_databases)
-
-    with db_out.open("w") as stream:
+    db_output = GLOBALS.RUNTIME_OUTPUT / "ioc.subst"
+    with db_output.open("w") as stream:
         stream.write(db_txt)
 
 
 def generate_pvi(ioc: IOC) -> Tuple[List[IndexEntry], List[Tuple[Database, Entity]]]:
     """Generate pvi bob and template files to add to UI index and IOC database.
 
     Args:
@@ -86,53 +77,57 @@
 
     formatted_pvi_devices: List[str] = []
     for entity in ioc.entities:
         entity_pvi = entity.__definition__.pvi
         if entity_pvi is None:
             continue
 
-        pvi_yaml = PVI_DEFS / entity_pvi.yaml_path
+        pvi_yaml = GLOBALS.PVI_DEFS / entity_pvi.yaml_path
         device_name = pvi_yaml.name.split(".")[0]
-        device_bob = OPI_OUTPUT_PATH / f"{device_name}.pvi.bob"
+        device_bob = GLOBALS.OPI_OUTPUT / f"{device_name}.pvi.bob"
 
         # Skip deserializing yaml if not needed
-        if entity_pvi.pva or device_name not in formatted_pvi_devices:
+        if entity_pvi.pv or device_name not in formatted_pvi_devices:
             device = Device.deserialize(pvi_yaml)
-            device.deserialize_parents([PVI_DEFS])
-
-            # render the prefix value for the device from the instance parameters
-            entity_dict = entity.model_dump()
-            prefix_value = render_with_utils(entity_dict, entity_pvi.prefix)
+            device.deserialize_parents([GLOBALS.PVI_DEFS])
 
-            macros = {"prefix": prefix_value}
-
-            if entity_pvi.pva:
+            if entity_pvi.pv:
                 # Create a template with the V4 structure defining a PVI interface
-                output_template = RUNTIME_OUTPUT_PATH / f"{device_name}.pvi.template"
-                format_template(device, PVI_PV_PREFIX, output_template)
+                output_template = GLOBALS.RUNTIME_OUTPUT / f"{device_name}.pvi.template"
+                format_template(device, entity_pvi.pv_prefix, output_template)
 
                 # Add to extra databases to be added into substitution file
                 databases.append(
-                    (Database(file=output_template.name, args=macros), entity)
+                    (
+                        Database(file=output_template.name, args=entity_pvi.ui_macros),
+                        entity,
+                    )
                 )
 
             if device_name not in formatted_pvi_devices:
-                formatter.format(device, PVI_PV_PREFIX, device_bob)
+                formatter.format(device, device_bob)
 
                 # Don't format further instance of this device
                 formatted_pvi_devices.append(device_name)
 
-        if entity_pvi.index:
-            index_entries.append(IndexEntry(device_name, device_bob.name, macros))
+        if entity_pvi.ui_index:
+            macros = UTILS.render_map(dict(entity), entity_pvi.ui_macros)
+            index_entries.append(
+                IndexEntry(
+                    label=f"{device.label}",
+                    ui=device_bob.name,
+                    macros=macros,
+                )
+            )
 
     return index_entries, databases
 
 
 def generate_index(title: str, index_entries: List[IndexEntry]):
     """Generate an index bob using pvi.
 
     Args:
         title: Title of index UI
         index_entries: List of entries to include as buttons on index UI
 
     """
-    DLSFormatter().format_index(title, index_entries, OPI_OUTPUT_PATH / "index.bob")
+    DLSFormatter().format_index(title, index_entries, GLOBALS.OPI_OUTPUT / "index.bob")
```

### Comparing `ibek-2023.11.1b5/src/ibek/support.py` & `ibek-3.4.0b2/src/ibek/support.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The Support Class represents a deserialized <MODULE_NAME>.ibek.support.yaml file.
 """
+
 from __future__ import annotations
 
 import json
 from enum import Enum
 from typing import Any, Dict, Mapping, Optional, Sequence, Union
 
 from pydantic import Field, PydanticUndefinedAnnotation
@@ -99,18 +100,23 @@
     A database file that should be loaded by the startup script and its args
     """
 
     file: str = Field(
         description="Filename of the database template in <module_root>/db"
     )
 
+    enabled: str = Field(
+        description="Set to False to disable loading this database", default="True"
+    )
+
     args: Mapping[str, Optional[str]] = Field(
         description=(
             "Dictionary of args and values to pass through to database. "
-            "A value of None is equivalent to ARG: '{{ ARG }}'"
+            "A value of None is equivalent to ARG: '{{ ARG }}'. "
+            "See `UTILS.render_map` for more details."
         )
     )
 
 
 class EnvironmentVariable(BaseSettings):
     """
     An environment variable that should be set in the startup script
@@ -158,21 +164,33 @@
 
 class EntityPVI(BaseSettings):
     """Entity PVI definition"""
 
     yaml_path: str = Field(
         description="Path to .pvi.device.yaml - absolute or relative to PVI_DEFS"
     )
-    index: bool = Field(
-        description="Whether to add generated UI to index for Entity", default=True
+    ui_index: bool = Field(
+        True,
+        description="Whether to add the UI to the IOC index.",
     )
-    prefix: str = Field(description="PV prefix to pass as $(prefix) on index button")
-    pva: bool = Field(
-        description="Whether to generate PVA structure template", default=False
+    ui_macros: dict[str, str | None] = Field(
+        None,
+        description=(
+            "Macros to launch the UI on the IOC index. "
+            "These must be args of the Entity this is attached to."
+        ),
+    )
+    pv: bool = Field(
+        False,
+        description=(
+            "Whether to generate a PVI PV. This adds a database template with info "
+            "tags that create a PVAccess PV representing the device structure."
+        ),
     )
+    pv_prefix: str = Field("", description='PV prefix for PVI PV - e.g. "$(P)"')
 
 
 class Definition(BaseSettings):
     """
     A single definition of a class of Entity that an IOC instance may instantiate
     """
```

### Comparing `ibek-2023.11.1b5/src/ibek/support_cmds/checks.py` & `ibek-3.4.0b2/src/ibek/support_cmds/checks.py`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/src/ibek/support_cmds/commands.py` & `ibek-3.4.0b2/src/ibek/support_cmds/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,29 @@
+import os
 import re
 import subprocess
 from enum import Enum
 from pathlib import Path
 from shutil import rmtree
 from typing import List, Optional
 
 import typer
 
-from ibek.ioc_cmds.assets import get_ioc_source
-
 try:
     from git import Repo
 except ImportError:
     pass  # Git Python is not needed for runtime (container build time only)
 
 from typing_extensions import Annotated
 
 from ibek.globals import (
-    IBEK_DEFS,
+    GLOBALS,
     IBEK_GLOBALS,
-    IBEK_SUPPORT,
     IOC_DBDS,
     IOC_LIBS,
-    PVI_DEFS,
     PVI_YAML_PATTERN,
     RELEASE,
     RUNTIME_DEBS,
     SUPPORT,
     SUPPORT_YAML_PATTERN,
     NaturalOrderGroup,
 )
@@ -55,54 +52,83 @@
 # only include values with at least one / (attempt to match filepaths only)
 PARSE_MACROS = re.compile(r"^([A-Z_a-z0-9]*)\s*=\s*(.*/.*)$", flags=re.M)
 
 
 support_cli = typer.Typer(cls=NaturalOrderGroup)
 
 
-@support_cli.command(
-    context_settings={"allow_extra_args": True, "ignore_unknown_options": True}
-)
-def apt_install(
-    ctx: typer.Context,
-    debs: List[str] = typer.Argument(None, help="list of debian packages to install"),
-    only: AptWhen = typer.Option(
-        AptWhen.both, help="which container build stage to install in"
-    ),
-    runtime: bool = typer.Option(False, help="install list of runtime packages"),
-):
+def _install_debs(debs: List[str]) -> None:
     """
-    Install debian packages into the container. If they have an http:// or https://
+    Install a list of debian packages.
+
+    If they have an http:// or https://
     prefix then they will be downloaded and installed from file.
     """
     temp = Path("/tmp")
-
-    if (only is AptWhen.run) or (only is AptWhen.both):
-        add_list_to_file(RUNTIME_DEBS, debs)
-    if only is AptWhen.run:
-        return
-
-    if runtime and RUNTIME_DEBS.exists():
-        debs += RUNTIME_DEBS.read_text().split()
-
     for i, pkg in enumerate(debs):
         if pkg.startswith("http://") or pkg.startswith("https://"):
             pkg_file = temp / pkg.split("/")[-1]
             subprocess.call(["wget", pkg, "-O", str(pkg_file)])
             debs[i] = str(pkg_file)
 
+    if len(debs) == 0:
+        print("no packages to install")
+        return
+
+    print("installing packages: ", debs)
+
+    sudo = "sudo" if os.geteuid() != 0 else ""
     command = (
-        "apt-get update && apt-get upgrade -y && "
-        "apt-get install -y --no-install-recommends "
-        + " ".join(debs)
-        + " ".join(ctx.args)
+        f"{sudo} apt-get update && {sudo} apt-get upgrade -y && "
+        f"{sudo} apt-get install -y --no-install-recommends " + " ".join(debs)
     )
     exit(subprocess.call(["bash", "-c", command]))
 
 
+@support_cli.command()
+def apt_install(
+    debs: List[str] = typer.Argument(None, help="list of debian packages to install"),
+):
+    """
+    Install packages
+    """
+    debs = debs or []
+    _install_debs(debs)
+
+
+@support_cli.command()
+def add_runtime_packages(
+    debs: List[str] = typer.Argument(None, help="list of debian packages to install"),
+):
+    """
+    Add packages to RUNTIME_DEBS for later install with apt_install_runtime_packages
+    """
+    debs = debs or []
+    add_list_to_file(RUNTIME_DEBS, debs)
+
+
+@support_cli.command()
+def apt_install_runtime_packages(
+    skip_non_native: bool = typer.Option(
+        False, help="skip installation in cross-compile environment"
+    ),
+):
+    """
+    Install packages from the list collected by calls to add_runtime_packages
+    """
+    if not GLOBALS.NATIVE and skip_non_native:
+        print("skipping runtime install in cross-compile environment")
+        return
+
+    if RUNTIME_DEBS.exists():
+        debs = RUNTIME_DEBS.read_text().split()
+
+    _install_debs(debs)
+
+
 @support_cli.command(
     context_settings={"allow_extra_args": True, "ignore_unknown_options": True}
 )
 def git_clone(
     ctx: typer.Context,
     repo_name: str = typer.Argument(..., help="repo to clone"),
     version: str = typer.Argument(..., help="tag to clone"),
@@ -126,15 +152,21 @@
         url, SUPPORT / repo_name, branch=version, depth=1, multi_options=ctx.args
     )
 
 
 @support_cli.command()
 def register(
     name: str = typer.Argument(..., help="the name of the support module"),
-    path: Annotated[Optional[Path], typer.Option(help="path to support module")] = None,
+    path: Annotated[
+        Optional[Path],
+        typer.Option(
+            help="path to support module",
+            autocompletion=lambda: [],  # Forces path autocompletion
+        ),
+    ] = None,
     macro: Optional[str] = typer.Option(None, help="Macro name for the module"),
 ):
     """
     prepare the configure RELEASE files to build a support module
     inside an epics-containers build
     """
     macro = name.upper() if macro is None else macro
@@ -157,24 +189,26 @@
 @support_cli.command()
 def add_libs(
     libs: List[str] = typer.Argument(None, help="list of libraries to add"),
 ) -> None:
     """
     declare the libraries for this support module for inclusion in IOC Makefile
     """
+    libs = libs or []
     add_list_to_file(IOC_LIBS, libs)
 
 
 @support_cli.command()
 def add_dbds(
     dbds: List[str] = typer.Argument(None, help="list of dbd files to add"),
 ) -> None:
     """
     declare the dbd files for this support module for inclusion in IOC Makefile
     """
+    dbds = dbds or []
     add_list_to_file(IOC_DBDS, dbds)
 
 
 @support_cli.command()
 def add_release_macro(
     macro: str = typer.Argument(..., help="macro name to update"),
     value: str = typer.Argument("", help="value to set for the macro"),
@@ -228,52 +262,55 @@
 ):
     """
     compile a support module after preparation with `ibek support register` etc.
     """
     path = SUPPORT / module
 
     command = f"make -C {path} -j $(nproc) " + " ".join(ctx.args)
-    exit(subprocess.call(["bash", "-c", command]))
+    result = subprocess.call(["bash", "-c", command])
+    # save size of developer container with make clean
+    command = f"make -C {path} -j $(nproc) clean"
+    subprocess.call(["bash", "-c", command])
+    exit(result)
 
 
 @support_cli.command()
 def generate_links(
-    support_module: Annotated[
+    folder: Annotated[
         Path,
         typer.Argument(
-            help="Support module to generate links for (directory in ibek-support)"
+            help="ibek-support(-xxx) folder to generate links for",
+            autocompletion=lambda: [],  # Forces path autocompletion
         ),
     ],
-    ibek_support: Annotated[
-        Optional[Path],
-        typer.Option(
-            help="Filepath to ibek-support root"
-            "defaults to <generic IOC source folder>/ibek-support"
-        ),
-    ] = None,
 ):
     """Generate symlinks to the ibek and pvi YAML files for a compiled IOC.
 
     Args:
-        support_module: Support module to generate links for
-        ibek_support: Root of ibek support to find support module directory in
-
-    """
-    support_defs = (ibek_support or get_ioc_source() / IBEK_SUPPORT) / support_module
-    support_globals = (ibek_support or get_ioc_source() / IBEK_SUPPORT) / IBEK_GLOBALS
-
-    symlink_files(support_defs, SUPPORT_YAML_PATTERN, IBEK_DEFS)
-    symlink_files(support_globals, SUPPORT_YAML_PATTERN, IBEK_DEFS)
-    symlink_files(support_defs, PVI_YAML_PATTERN, PVI_DEFS)
+        folder: path to an ibek-support folder containing the YAML files
+                for the support module to link to. This should be a sub
+                module of the ioc-xxx Generic IOC project and may be the
+                public ibek-support repo or a private ibek-support-xxx repo.
+    """
+    support_globals = folder / ".." / IBEK_GLOBALS
+
+    symlink_files(folder, SUPPORT_YAML_PATTERN, GLOBALS.IBEK_DEFS)
+    if support_globals.exists():
+        symlink_files(support_globals, SUPPORT_YAML_PATTERN, GLOBALS.IBEK_DEFS)
+    symlink_files(folder, PVI_YAML_PATTERN, GLOBALS.PVI_DEFS)
 
 
 @support_cli.command()
 def generate_schema(
     output: Annotated[
-        Optional[Path], typer.Option(help="The filename to write the schema to")
+        Optional[Path],
+        typer.Option(
+            help="The filename to write the schema to",
+            autocompletion=lambda: [],  # Forces path autocompletion
+        ),
     ] = None,
 ):
     """Produce JSON global schema for all <support_module>.ibek.support.yaml files"""
     if output is None:
         typer.echo(Support.get_schema())
     else:
         output.write_text(Support.get_schema())
```

### Comparing `ibek-2023.11.1b5/src/ibek.egg-info/PKG-INFO` & `ibek-3.4.0b2/src/ibek.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibek
-Version: 2023.11.1b5
+Version: 3.4.0b2
 Summary: IOC Builder for EPICS and Kubernetes
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,30 +209,29 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: pydantic==2.3.0
+Requires-Dist: pydantic==2.6.4
 Requires-Dist: typer
 Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2
 Requires-Dist: GitPython
-Requires-Dist: pvi>=0.6
+Requires-Dist: pvi~=0.8
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pipdeptree; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pydata-sphinx-theme>=0.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
-Requires-Dist: pytest-env; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: Sphinx==6.2.1; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinx-design; extra == "dev"
 Requires-Dist: tox-direct; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
@@ -244,14 +243,15 @@
 
 
 This tool supports building container images for Generic EPICS IOCs and
 generating IOC Instances from those Generic IOCs at container runtime. It is
 targetted at running IOCs in Kubernetes, but the images it
 creates can execute in any container runtime, such as docker or podman.
 
+
   ============== ==============================================================
   PyPI           ``pip install ibek``
   Source code    https://github.com/epics-containers/ibek
   Documentation  https://epics-containers.github.io/ibek
   Releases       https://github.com/epics-containers/ibek/releases
   ============== ==============================================================
```

### Comparing `ibek-2023.11.1b5/src/ibek.egg-info/SOURCES.txt` & `ibek-3.4.0b2/src/ibek.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 .github/dependabot.yml
 .github/actions/install_requirements/action.yml
 .github/pages/index.html
 .github/pages/make_switcher.py
 .github/workflows/code.yml
 .github/workflows/docs.yml
 .github/workflows/docs_clean.yml
-.github/workflows/linkcheck.yml
 .vscode/extensions.json
 .vscode/launch.json
 .vscode/settings.json
 .vscode/tasks.json
 docs/conf.py
 docs/genindex.rst
 docs/index.rst
@@ -69,72 +68,57 @@
 src/ibek/utils.py
 src/ibek.egg-info/PKG-INFO
 src/ibek.egg-info/SOURCES.txt
 src/ibek.egg-info/dependency_links.txt
 src/ibek.egg-info/entry_points.txt
 src/ibek.egg-info/requires.txt
 src/ibek.egg-info/top_level.txt
+src/ibek/dev_cmds/__init__.py
+src/ibek/dev_cmds/commands.py
 src/ibek/ioc_cmds/__init__.py
 src/ibek/ioc_cmds/assets.py
 src/ibek/ioc_cmds/commands.py
 src/ibek/ioc_cmds/docker.py
 src/ibek/runtime_cmds/__init__.py
 src/ibek/runtime_cmds/commands.py
 src/ibek/support_cmds/__init__.py
 src/ibek/support_cmds/checks.py
 src/ibek/support_cmds/commands.py
 src/ibek/support_cmds/files.py
 src/ibek/templates/ioc.subst.jinja
 src/ibek/templates/st.cmd.jinja
-src/ibek/templates/ioc/Makefile
-src/ibek/templates/ioc/liveness.sh
-src/ibek/templates/ioc/start.sh
-src/ibek/templates/ioc/stop.sh
-src/ibek/templates/ioc/config/start.sh
-src/ibek/templates/ioc/configure/CONFIG
-src/ibek/templates/ioc/configure/CONFIG_SITE
-src/ibek/templates/ioc/configure/Makefile
-src/ibek/templates/ioc/configure/RELEASE
-src/ibek/templates/ioc/configure/RULES
-src/ibek/templates/ioc/configure/RULES.ioc
-src/ibek/templates/ioc/configure/RULES_DIRS
-src/ibek/templates/ioc/configure/RULES_TOP
-src/ibek/templates/ioc/iocApp/src/Makefile.jinja
-src/ibek/templates/ioc/iocApp/src/iocMain.cpp
 src/ibek/templates/support/Makefile
 src/ibek/templates/support/configure/RELEASE
 tests/__init__.py
 tests/conftest.py
 tests/generate_samples.sh
 tests/sys-test.sh
 tests/test_cli.py
 tests/test_error.py
 tests/test_render.py
 tests/test_support.py
 tests/test_unit.py
 tests/samples/epics/pvi-defs/simple.pvi.device.yaml
-tests/samples/outputs/all.ioc.subst
-tests/samples/outputs/all.st.cmd
-tests/samples/outputs/index.bob
-tests/samples/outputs/objects.ioc.subst
-tests/samples/outputs/objects.st.cmd
-tests/samples/outputs/simple.pvi.bob
-tests/samples/outputs/simple.pvi.template
-tests/samples/outputs/utils.ioc.subst
-tests/samples/outputs/utils.st.cmd
+tests/samples/iocs/bad_counter.ibek.ioc.yaml
+tests/samples/iocs/bad_counter2.ibek.ioc.yaml
+tests/samples/iocs/bad_db.ibek.ioc.yaml
+tests/samples/iocs/bad_default.ibek.ioc.yaml
+tests/samples/iocs/bad_ref.ibek.ioc.yaml
+tests/samples/iocs/ibek-mo-ioc-01.yaml
+tests/samples/iocs/utils.ibek.ioc.yaml
+tests/samples/outputs/motorSim/index.bob
+tests/samples/outputs/motorSim/ioc.subst
+tests/samples/outputs/motorSim/simple.pvi.bob
+tests/samples/outputs/motorSim/simple.pvi.template
+tests/samples/outputs/motorSim/st.cmd
+tests/samples/outputs/utils/index.bob
+tests/samples/outputs/utils/ioc.subst
+tests/samples/outputs/utils/st.cmd
 tests/samples/schemas/ibek.support.schema.json
-tests/samples/schemas/multiple.ibek.ioc.schema.json
-tests/samples/schemas/objects.ibek.ioc.schema.json
+tests/samples/schemas/motorSim.ibek.ioc.schema.json
+tests/samples/schemas/single.ibek.ioc.schema.json
 tests/samples/schemas/utils.ibek.ioc.schema.json
-tests/samples/yaml/all.ibek.ioc.yaml
-tests/samples/yaml/all.ibek.support.yaml
-tests/samples/yaml/bad_counter.ibek.ioc.yaml
-tests/samples/yaml/bad_counter2.ibek.ioc.yaml
-tests/samples/yaml/bad_db.ibek.ioc.yaml
-tests/samples/yaml/bad_db.ibek.support.yaml
-tests/samples/yaml/bad_default.ibek.ioc.yaml
-tests/samples/yaml/bad_ref.ibek.ioc.yaml
-tests/samples/yaml/objects.ibek.ioc.yaml
-tests/samples/yaml/objects.ibek.support.yaml
-tests/samples/yaml/simple.pvi.device.yaml
-tests/samples/yaml/utils.ibek.ioc.yaml
-tests/samples/yaml/utils.ibek.support.yaml
+tests/samples/support/asyn.ibek.support.yaml
+tests/samples/support/bad_db.ibek.support.yaml
+tests/samples/support/motorSim.ibek.support.yaml
+tests/samples/support/simple.pvi.device.yaml
+tests/samples/support/utils.ibek.support.yaml
```

### Comparing `ibek-2023.11.1b5/tests/conftest.py` & `ibek-3.4.0b2/tests/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import os
 from pathlib import Path
 
 from pytest import fixture
 from ruamel.yaml import YAML
 from typer.testing import CliRunner
 
+# This must be above the following imports so that it takes effect before
+# `globals.EPICS_ROOT` is imported (or anything built on top of it)
 os.environ["EPICS_ROOT"] = str(Path(__file__).parent / "samples" / "epics")
 
+# The `noqa`s on these imports are necessary because of the above
 from ibek.__main__ import cli  # noqa: E402
 from ibek.ioc import clear_entity_model_ids, make_entity_models  # noqa: E402
 from ibek.support import Support  # noqa: E402
 
 runner = CliRunner()
 
 
@@ -39,42 +42,46 @@
 
 @fixture
 def samples():
     return Path(__file__).parent / "samples"
 
 
 @fixture
-def yaml_defs(samples):
-    return samples / "yaml"
+def support_defs(samples):
+    return samples / "support"
 
 
 @fixture
-def objects_classes(yaml_defs):
+def ioc_defs(samples):
+    return samples / "iocs"
+
+
+@fixture
+def asyn_classes(support_defs):
     # clear the entity classes to make sure there's nothing left
     clear_entity_model_ids()
 
-    objects_support = get_support(yaml_defs / "objects.ibek.support.yaml")
+    asyn_support = get_support(support_defs / "asyn.ibek.support.yaml")
 
     # make entity subclasses for everything defined in it
-    namespace = make_entity_models(objects_support)
+    namespace = make_entity_models(asyn_support)
 
     # return the namespace so that callers have access to all of the
     # generated dataclasses
     return namespace
 
 
 @fixture
-def epics_support(ibek_defs):
-    return get_support(ibek_defs / "_global", "epics.ibek.support.yaml")
-
-
-@fixture
-def epics_classes(epics_support):
+def motor_classes(support_defs):
     # clear the entity classes to make sure there's nothing left
     clear_entity_model_ids()
 
+    asyn_support = get_support(support_defs / "asyn.ibek.support.yaml")
+    motor_support = get_support(support_defs / "motorSim.ibek.support.yaml")
+
     # make entity subclasses for everything defined in it
-    namespace = make_entity_models(epics_support)
+    namespace = make_entity_models(asyn_support)
+    namespace.extend(make_entity_models(motor_support))
 
     # return the namespace so that callers have access to all of the
     # generated dataclasses
     return namespace
```

### Comparing `ibek-2023.11.1b5/tests/generate_samples.sh` & `ibek-3.4.0b2/tests/generate_samples.sh`

 * *Files 22% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 # please bear in mind that this is cheating tests! It requires visual
 # verifiction of the files in the samples folders after running.
 #
 
 export SAMPLES_DIR=$(realpath $(dirname "${BASH_SOURCE[0]}"))/samples
 
 export EPICS_ROOT=${SAMPLES_DIR}/epics
+export IOC="/epics/ioc"
+export RUNTIME_DIR="/epics/runtime"
 
 # this is so relative schema mode lines work
 cd $SAMPLES_DIR
 mkdir -p schemas
 mkdir -p outputs
 
 set -ex
 
 mkdir -p epics/pvi-defs
-cp yaml/simple.pvi.device.yaml  epics/pvi-defs/simple.pvi.device.yaml
+cp support/simple.pvi.device.yaml  epics/pvi-defs/simple.pvi.device.yaml
 
 echo making the support yaml schema
 ibek support generate-schema --output schemas/ibek.support.schema.json
 
-echo making an ioc schema using object support yaml
-ibek ioc generate-schema yaml/objects.ibek.support.yaml --output schemas/objects.ibek.ioc.schema.json
+echo making an ioc schema using just motorSim support yaml
+ibek ioc generate-schema --no-ibek-defs support/motorSim.ibek.support.yaml --output schemas/single.ibek.ioc.schema.json
 
-echo making an ioc schema using utils support yaml
-ibek ioc generate-schema yaml/utils.ibek.support.yaml --output schemas/utils.ibek.ioc.schema.json
+echo making an ioc schema using motorSim and Asyn support yaml
+ibek ioc generate-schema --no-ibek-defs support/asyn.ibek.support.yaml support/motorSim.ibek.support.yaml --output schemas/motorSim.ibek.ioc.schema.json
 
-echo making an ioc schema using multiple support yaml files
-ibek ioc generate-schema yaml/objects.ibek.support.yaml yaml/all.ibek.support.yaml --output schemas/multiple.ibek.ioc.schema.json
+echo making an ioc schema using utils support yaml
+ibek ioc generate-schema --no-ibek-defs support/utils.ibek.support.yaml --output schemas/utils.ibek.ioc.schema.json
 
-echo making ioc based on objects support yaml
-ibek runtime generate yaml/objects.ibek.ioc.yaml yaml/objects.ibek.support.yaml --out outputs/objects.st.cmd --db-out outputs/objects.ioc.subst
+echo making ioc based on ibek-mo-ioc-01.yaml
+EPICS_ROOT=`pwd`/epics ibek runtime generate iocs/ibek-mo-ioc-01.yaml support/asyn.ibek.support.yaml support/motorSim.ibek.support.yaml
+mv `pwd`/epics/{runtime,opi}/* `pwd`/outputs/motorSim
 
 echo making ioc based on utils support yaml
-ibek runtime generate yaml/utils.ibek.ioc.yaml yaml/utils.ibek.support.yaml --out outputs/utils.st.cmd --db-out outputs/utils.ioc.subst
-
-echo making ioc based on mutiple support yaml
-ibek runtime generate yaml/all.ibek.ioc.yaml yaml/objects.ibek.support.yaml yaml/all.ibek.support.yaml --out outputs/all.st.cmd --db-out outputs/all.ioc.subst
-cp epics/opi/* outputs/
+EPICS_ROOT=`pwd`/epics ibek runtime generate iocs/utils.ibek.ioc.yaml support/utils.ibek.support.yaml
+mv `pwd`/epics/{runtime,opi}/* `pwd`/outputs/utils
```

### Comparing `ibek-2023.11.1b5/tests/samples/outputs/simple.pvi.bob` & `ibek-3.4.0b2/tests/samples/outputs/motorSim/index.bob`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 <display version="2.0.0">
   <name>Display</name>
   <x>0</x>
-  <y>0</y>
-  <width>273</width>
+  <y use_class="true">0</y>
+  <width>388</width>
   <height>55</height>
   <grid_step_x>4</grid_step_x>
   <grid_step_y>4</grid_step_y>
   <widget type="label" version="2.0.0">
     <name>Title</name>
     <class>TITLE</class>
-    <text>Simple Device - ${prefix}</text>
+    <text>ibek-mo-ioc-01</text>
     <x use_class="true">0</x>
     <y use_class="true">0</y>
-    <width>273</width>
+    <width>388</width>
     <height>25</height>
     <font use_class="true">
       <font name="Header 1" family="Liberation Sans" style="BOLD" size="22.0">
       </font>
     </font>
     <foreground_color use_class="true">
       <color name="Text" red="0" green="0" blue="0">
       </color>
     </foreground_color>
     <transparent use_class="true">true</transparent>
     <horizontal_alignment>1</horizontal_alignment>
   </widget>
   <widget type="label" version="2.0.0">
     <name>Label</name>
-    <text>Simple PV</text>
+    <text>Simple Device</text>
     <x>23</x>
     <y>30</y>
-    <width>115</width>
+    <width>150</width>
     <height>20</height>
   </widget>
-  <widget type="textupdate" version="2.0.0">
-    <name>TextUpdate</name>
-    <pv_name>${prefix}Simple</pv_name>
-    <x>143</x>
+  <widget type="action_button" version="3.0.0">
+    <name>OpenDisplay</name>
+    <actions>
+      <action type="open_display">
+        <file>simple.pvi.bob</file>
+        <target>tab</target>
+        <description>Open Display</description>
+        <macros>
+          <P>IBEK-MO-TST-01:</P>
+        </macros>
+      </action>
+    </actions>
+    <text>IBEK-MO-TST-01:</text>
+    <x>178</x>
     <y>30</y>
-    <width>125</width>
+    <width>205</width>
     <height>20</height>
-    <font>
-      <font name="Default Bold" family="Liberation Sans" style="BOLD" size="14.0">
-      </font>
-    </font>
-    <horizontal_alignment>1</horizontal_alignment>
+    <tooltip>$(actions)</tooltip>
   </widget>
 </display>
```

### Comparing `ibek-2023.11.1b5/tests/samples/schemas/ibek.support.schema.json` & `ibek-3.4.0b2/tests/samples/schemas/ibek.support.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996569113756614%*

 * *Differences: {"'$defs'": '{\'Database\': {\'properties\': {\'args\': {\'description\': "Dictionary of args and '*

 * *            "values to pass through to database. A value of None is equivalent to ARG: '{{ ARG "*

 * *            '}}\'. See `UTILS.render_map` for more details."}, \'enabled\': '*

 * *            "OrderedDict([('default', 'True'), ('description', 'Set to False to disable loading "*

 * *            "this database'), ('title', 'Enabled'), ('type', 'string')])}}, 'EntityPVI': "*

 * *            "{'properties': {'ui_index': Ordered […]*

```diff
@@ -78,18 +78,24 @@
                                 "type": "string"
                             },
                             {
                                 "type": "null"
                             }
                         ]
                     },
-                    "description": "Dictionary of args and values to pass through to database. A value of None is equivalent to ARG: '{{ ARG }}'",
+                    "description": "Dictionary of args and values to pass through to database. A value of None is equivalent to ARG: '{{ ARG }}'. See `UTILS.render_map` for more details.",
                     "title": "Args",
                     "type": "object"
                 },
+                "enabled": {
+                    "default": "True",
+                    "description": "Set to False to disable loading this database",
+                    "title": "Enabled",
+                    "type": "string"
+                },
                 "file": {
                     "description": "Filename of the database template in <module_root>/db",
                     "title": "File",
                     "type": "string"
                 }
             },
             "required": [
@@ -220,40 +226,56 @@
             "title": "Definition",
             "type": "object"
         },
         "EntityPVI": {
             "additionalProperties": false,
             "description": "Entity PVI definition",
             "properties": {
-                "index": {
-                    "default": true,
-                    "description": "Whether to add generated UI to index for Entity",
-                    "title": "Index",
+                "pv": {
+                    "default": false,
+                    "description": "Whether to generate a PVI PV. This adds a database template with info tags that create a PVAccess PV representing the device structure.",
+                    "title": "Pv",
                     "type": "boolean"
                 },
-                "prefix": {
-                    "description": "PV prefix to pass as $(prefix) on index button",
-                    "title": "Prefix",
+                "pv_prefix": {
+                    "default": "",
+                    "description": "PV prefix for PVI PV - e.g. \"$(P)\"",
+                    "title": "Pv Prefix",
                     "type": "string"
                 },
-                "pva": {
-                    "default": false,
-                    "description": "Whether to generate PVA structure template",
-                    "title": "Pva",
+                "ui_index": {
+                    "default": true,
+                    "description": "Whether to add the UI to the IOC index.",
+                    "title": "Ui Index",
                     "type": "boolean"
                 },
+                "ui_macros": {
+                    "additionalProperties": {
+                        "anyOf": [
+                            {
+                                "type": "string"
+                            },
+                            {
+                                "type": "null"
+                            }
+                        ]
+                    },
+                    "default": null,
+                    "description": "Macros to launch the UI on the IOC index. These must be args of the Entity this is attached to.",
+                    "title": "Ui Macros",
+                    "type": "object"
+                },
                 "yaml_path": {
                     "description": "Path to .pvi.device.yaml - absolute or relative to PVI_DEFS",
                     "title": "Yaml Path",
                     "type": "string"
                 }
             },
             "required": [
-                "yaml_path",
-                "prefix"
+                "yaml_path"
             ],
             "title": "EntityPVI",
             "type": "object"
         },
         "EnumArg": {
             "additionalProperties": false,
             "description": "An argument with an enum value",
```

### Comparing `ibek-2023.11.1b5/tests/samples/schemas/multiple.ibek.ioc.schema.json` & `ibek-3.4.0b2/tests/samples/schemas/single.ibek.ioc.schema.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9149305555555555%*

 * *Differences: {"'$defs'": "{replace: OrderedDict([('DIR', OrderedDict([('enum', ['Pos', 'Neg']), ('title', "*

 * *            "'DIR'), ('type', 'string')])), ('motorSim_simMotorAxis', "*

 * *            "OrderedDict([('additionalProperties', False), ('properties', OrderedDict([('type', "*

 * *            "OrderedDict([('const', 'motorSim.simMotorAxis'), ('default', "*

 * *            "'motorSim.simMotorAxis'), ('description', 'The type of this entity'), ('title', "*

 * *            "'Type')])), ('entity_enabled', OrderedDict([('default', True),  […]*

```diff
@@ -1,254 +1,192 @@
 {
     "$defs": {
-        "clock_rate": {
+        "DIR": {
             "enum": [
-                "1Hz",
-                "2Hz",
-                "5Hz",
-                "10Hz",
-                "dummy"
+                "Pos",
+                "Neg"
             ],
-            "title": "clock_rate",
+            "title": "DIR",
             "type": "string"
         },
-        "module_AllObject": {
+        "motorSim_simMotorAxis": {
             "additionalProperties": false,
             "properties": {
-                "calculated_one": {
-                    "default": "{{ name }}.{{ my_str }}.{{ my_int }}.{{ my_float }}.{{ my_bool }}",
-                    "description": "test jinja render of arg values",
-                    "title": "Calculated One",
-                    "type": "string"
-                },
-                "clock_rate": {
-                    "allOf": [
-                        {
-                            "$ref": "#/$defs/clock_rate"
-                        }
-                    ],
-                    "description": "demonstrates use of VME clock rates as an enum\nthis is an example of an 'illegal' python enum\n"
+                "ADDR": {
+                    "description": "The axis number (allowed to be from 0 to controller.numAxes-1)",
+                    "title": "Addr",
+                    "type": "integer"
                 },
-                "entity_enabled": {
-                    "default": true,
-                    "description": "enable or disable this entity instance",
-                    "title": "Entity Enabled",
-                    "type": "boolean"
+                "CS_NUM": {
+                    "default": 0,
+                    "description": "The coordinate system number for this axis",
+                    "title": "Cs Num",
+                    "type": "integer"
                 },
-                "my_bool": {
-                    "default": true,
-                    "description": "bool arg",
-                    "title": "My Bool",
-                    "type": "boolean"
+                "DESC": {
+                    "default": "Motor {{ADDR}}",
+                    "description": "The description of the axis",
+                    "title": "Desc",
+                    "type": "string"
                 },
-                "my_float": {
-                    "default": 1.0,
-                    "description": "float arg",
-                    "title": "My Float",
-                    "type": "number"
+                "DHLM": {
+                    "default": 20000,
+                    "description": "The high limit of the axis (in counts)",
+                    "title": "Dhlm",
+                    "type": "integer"
                 },
-                "my_inferred_enum": {
+                "DIR": {
                     "allOf": [
                         {
-                            "$ref": "#/$defs/my_inferred_enum"
+                            "$ref": "#/$defs/DIR"
                         }
                     ],
-                    "description": "integer enumerated type with inferred value"
+                    "default": 0,
+                    "description": "The direction of the axis"
                 },
-                "my_int": {
-                    "default": 1,
-                    "description": "integer arg",
-                    "title": "My Int",
+                "DLLM": {
+                    "default": -20000,
+                    "description": "The low limit of the axis (in counts)",
+                    "title": "Dllm",
                     "type": "integer"
                 },
-                "my_int_enum": {
-                    "allOf": [
-                        {
-                            "$ref": "#/$defs/my_int_enum"
-                        }
-                    ],
-                    "default": 2,
-                    "description": "integer enumerated type"
+                "M": {
+                    "description": "PV suffix for the motor record",
+                    "title": "M",
+                    "type": "string"
                 },
-                "my_object": {
-                    "description": "object arg",
-                    "title": "My Object"
+                "VELO": {
+                    "default": 10.0,
+                    "description": "The velocity of the axis (in counts/sec)",
+                    "title": "Velo",
+                    "type": "number"
                 },
-                "my_str": {
-                    "description": "string arg",
-                    "title": "My Str",
+                "VMAX": {
+                    "default": "{{VELO}}",
+                    "description": "The maximum velocity of the axis (in counts/sec)",
+                    "title": "Vmax",
                     "type": "string"
                 },
-                "name": {
-                    "description": "identifier",
-                    "title": "Name",
-                    "type": "string"
-                },
-                "type": {
-                    "const": "module.AllObject",
-                    "default": "module.AllObject",
-                    "description": "The type of this entity",
-                    "title": "Type"
-                }
-            },
-            "required": [
-                "name",
-                "my_inferred_enum",
-                "clock_rate",
-                "my_str",
-                "my_object"
-            ],
-            "title": "module_AllObject",
-            "type": "object"
-        },
-        "my_inferred_enum": {
-            "enum": [
-                "first",
-                "second",
-                "third"
-            ],
-            "title": "my_inferred_enum",
-            "type": "string"
-        },
-        "my_int_enum": {
-            "enum": [
-                "all_ahead",
-                "full_speed",
-                "ramming_speed",
-                "stop"
-            ],
-            "title": "my_int_enum",
-            "type": "string"
-        },
-        "object_module_Consumer": {
-            "additionalProperties": false,
-            "properties": {
-                "PORT": {
-                    "description": "a reference to an RefObject",
-                    "title": "Port"
+                "controller": {
+                    "description": "a reference to the motion controller",
+                    "title": "Controller"
                 },
                 "entity_enabled": {
                     "default": true,
                     "description": "enable or disable this entity instance",
                     "title": "Entity Enabled",
                     "type": "boolean"
                 },
-                "name": {
-                    "description": "Consumer name",
-                    "title": "Name",
-                    "type": "string"
-                },
-                "type": {
-                    "const": "object_module.Consumer",
-                    "default": "object_module.Consumer",
-                    "description": "The type of this entity",
-                    "title": "Type"
-                }
-            },
-            "required": [
-                "name",
-                "PORT"
-            ],
-            "title": "object_module_Consumer",
-            "type": "object"
-        },
-        "object_module_ConsumerTwo": {
-            "additionalProperties": false,
-            "properties": {
-                "PORT": {
-                    "description": "a reference to an RefObject",
-                    "title": "Port"
+                "home": {
+                    "default": 0,
+                    "description": "The home position of the axis (in counts)",
+                    "title": "Home",
+                    "type": "integer"
                 },
-                "entity_enabled": {
-                    "default": true,
-                    "description": "enable or disable this entity instance",
-                    "title": "Entity Enabled",
+                "is_cs": {
+                    "default": false,
+                    "description": "Set to True if this axis a coordinate system axis",
+                    "title": "Is Cs",
                     "type": "boolean"
                 },
-                "name": {
-                    "description": "Consumer name",
-                    "title": "Name",
+                "start": {
+                    "default": "{{home}}",
+                    "description": "The starting position of the axis (in counts)",
+                    "title": "Start",
                     "type": "string"
                 },
                 "type": {
-                    "const": "object_module.ConsumerTwo",
-                    "default": "object_module.ConsumerTwo",
+                    "const": "motorSim.simMotorAxis",
+                    "default": "motorSim.simMotorAxis",
                     "description": "The type of this entity",
                     "title": "Type"
                 }
             },
             "required": [
-                "name",
-                "PORT"
+                "controller",
+                "M",
+                "ADDR"
             ],
-            "title": "object_module_ConsumerTwo",
+            "title": "motorSim_simMotorAxis",
             "type": "object"
         },
-        "object_module_RefObject": {
+        "motorSim_simMotorController": {
             "additionalProperties": false,
             "properties": {
-                "IP": {
-                    "default": "127.0.0.1",
-                    "description": "IP address of port",
-                    "title": "Ip",
+                "DESC": {
+                    "default": "Simulated Motion Controller testing escaping: {% raw %} {{enclosed in escaped curly braces}} {% endraw %}",
+                    "description": "The description of the controller",
+                    "title": "Desc",
+                    "type": "string"
+                },
+                "P": {
+                    "description": "Device PV Prefix",
+                    "title": "P",
+                    "type": "string"
+                },
+                "controllerName": {
+                    "description": "The name of the controller and its Asyn Port Name",
+                    "title": "Controllername",
                     "type": "string"
                 },
                 "entity_enabled": {
                     "default": true,
                     "description": "enable or disable this entity instance",
                     "title": "Entity Enabled",
                     "type": "boolean"
                 },
-                "name": {
-                    "description": "Port name",
-                    "title": "Name",
-                    "type": "string"
+                "numAxes": {
+                    "description": "The number of axes to create",
+                    "title": "Numaxes",
+                    "type": "integer"
                 },
-                "test_value": {
-                    "default": "{{ name }}.{{ IP }}",
-                    "description": "test jinja render of arg values",
-                    "title": "Test Value",
-                    "type": "string"
+                "port": {
+                    "description": "a reference to the asyn port for communication with the controller",
+                    "title": "Port"
                 },
                 "type": {
-                    "const": "object_module.RefObject",
-                    "default": "object_module.RefObject",
+                    "const": "motorSim.simMotorController",
+                    "default": "motorSim.simMotorController",
                     "description": "The type of this entity",
                     "title": "Type"
                 }
             },
             "required": [
-                "name"
+                "controllerName",
+                "P",
+                "numAxes",
+                "port"
             ],
-            "title": "object_module_RefObject",
+            "title": "motorSim_simMotorController",
             "type": "object"
         }
     },
     "additionalProperties": false,
     "properties": {
         "description": {
             "description": "Description of what the IOC does",
             "title": "Description",
             "type": "string"
         },
         "entities": {
             "description": "List of entities this IOC instantiates",
             "items": {
-                "anyOf": [
-                    {
-                        "$ref": "#/$defs/object_module_RefObject"
-                    },
-                    {
-                        "$ref": "#/$defs/object_module_Consumer"
+                "discriminator": {
+                    "mapping": {
+                        "motorSim.simMotorAxis": "#/$defs/motorSim_simMotorAxis",
+                        "motorSim.simMotorController": "#/$defs/motorSim_simMotorController"
                     },
+                    "propertyName": "type"
+                },
+                "oneOf": [
                     {
-                        "$ref": "#/$defs/object_module_ConsumerTwo"
+                        "$ref": "#/$defs/motorSim_simMotorController"
                     },
                     {
-                        "$ref": "#/$defs/module_AllObject"
+                        "$ref": "#/$defs/motorSim_simMotorAxis"
                     }
                 ]
             },
             "title": "Entities",
             "type": "array"
         },
         "ioc_name": {
```

### Comparing `ibek-2023.11.1b5/tests/samples/schemas/utils.ibek.ioc.schema.json` & `ibek-3.4.0b2/tests/samples/schemas/utils.ibek.ioc.schema.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982638888888888%*

 * *Differences: {"'properties'": "{'entities': {'items': {replace: OrderedDict([('discriminator', "*

 * *                 "OrderedDict([('mapping', OrderedDict([('epics.InterruptVectorVME', "*

 * *                 "'#/$defs/epics_InterruptVectorVME'), ('epics.InterruptVectorVME2', "*

 * *                 "'#/$defs/epics_InterruptVectorVME2')])), ('propertyName', 'type')])), ('oneOf', "*

 * *                 "[OrderedDict([('$ref', '#/$defs/epics_InterruptVectorVME')]), "*

 * *                 "OrderedDict([('$ref', '#/$defs/epics_InterruptVectorVM […]*

```diff
@@ -73,15 +73,22 @@
             "description": "Description of what the IOC does",
             "title": "Description",
             "type": "string"
         },
         "entities": {
             "description": "List of entities this IOC instantiates",
             "items": {
-                "anyOf": [
+                "discriminator": {
+                    "mapping": {
+                        "epics.InterruptVectorVME": "#/$defs/epics_InterruptVectorVME",
+                        "epics.InterruptVectorVME2": "#/$defs/epics_InterruptVectorVME2"
+                    },
+                    "propertyName": "type"
+                },
+                "oneOf": [
                     {
                         "$ref": "#/$defs/epics_InterruptVectorVME"
                     },
                     {
                         "$ref": "#/$defs/epics_InterruptVectorVME2"
                     }
                 ]
```

### Comparing `ibek-2023.11.1b5/tests/samples/yaml/bad_db.ibek.support.yaml` & `ibek-3.4.0b2/tests/samples/support/bad_db.ibek.support.yaml`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/tests/samples/yaml/objects.ibek.support.yaml` & `ibek-3.4.0b2/tests/samples/support/asyn.ibek.support.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,121 @@
-# yaml-language-server: $schema=../schemas/ibek.support.schema.json
+# yaml-language-server: $schema=https://github.com/epics-containers/ibek/releases/download/1.5.3/ibek.support.schema.json
 
-################################################################################
-### ibek support YAML to demonstrate the use of object references
-################################################################################
-module: object_module
+module: asyn
 
 defs:
-  - name: RefObject
-    description: |
-      Example object for reference from Consumer
+  - name: AsynIP
+    description: |-
+      Asyn IP Port
     args:
+      - type: str
+        name: port
+        description: |-
+          Serial port tty name / IP address optionally followed by protocol
+
       - type: id
         name: name
-        description: Port name
+        description: |-
+          Override name
 
       - type: str
-        name: IP
-        description: IP address of port
-        default: 127.0.0.1
-
-    values:
-      - name: test_value
-        value: "{{ name }}.{{ IP }}"
-        description: test jinja render of arg values
+        name: input_eos
+        description: |-
+          Input end of string (terminator)
+        # test escaping of quotes
+        default: '"\n"'
 
+      - type: str
+        name: output_eos
+        description: |-
+          Output end of string (terminator)
+        default: '"\n"'
+
+      - type: int
+        name: priority
+        description: |-
+          Priority
+        default: 100
+
+      - type: bool
+        name: noAuto_connect
+        description: |-
+          Set to stop auto_connect
+        default: false
+
+      - type: bool
+        name: noProcessEos
+        description: |-
+          Set to avoid processing end of string
+        default: false
+
+      - type: int
+        name: baud
+        description: |-
+          Baud Rate
+        default: 9600
+
+      - type: enum
+        name: parity
+        description: |-
+          Parity
+        values:
+          even:
+          none:
+          odd:
+        default: none
+
+      - type: enum
+        name: crtscts
+        description: |-
+          Set hardware flow control on
+        values:
+          Y:
+          N:
+        default: N
+
+      - type: enum
+        name: stop
+        description: |-
+          Stop Bits
+        values:
+          "1":
+          "2":
+        default: "1"
+
+      - type: enum
+        name: disconnectOnReadTimeout
+        description: |-
+          Disconnect when a read times out
+        values:
+          Y:
+          N:
+        default: Y
+
+      - type: enum
+        name: bits
+        description: |-
+          Bits
+        values:
+          "8":
+          "5":
+          "7":
+          "6":
+        default: "8"
+
+    # test environment variables declaration
     env_vars:
-      - name: REF_OBJECT_NAME
-        value: "{{ name }}"
+      - name: NAME_AS_ENV_VAR
+        value: "my name is {{ name }}"
 
     pre_init:
+      - value: |
+          # Setting up Asyn Port {{name}} on {{port}}:
       - when: first
+        # test escaping of jinja directives and use of 'first' to only print this line once
         value: |
-          # This line should appear once only in the pre_init section
-      - value: |
-          # TestValues testValue
-          TestValues {{ test_value }}
-
-    pvi:
-      yaml_path: simple.pvi.device.yaml
-      prefix: "{{ name }}"
-
-  - name: Consumer
-    description: |
-      A class that uses RefObject
-    args:
-      - type: id
-        name: name
-        description: Consumer name
-
-      - type: object
-        name: PORT
-        description: a reference to an RefObject
-
-  - name: ConsumerTwo
-    description: |
-      Another class that uses RefObject
-    args:
-      - type: id
-        name: name
-        description: Consumer name
-
-      - type: object
-        name: PORT
-        description: a reference to an RefObject
-
-    pre_init:
+          # {% raw %}AsynIPConfigure({{name}}, {{port}}, {{stop}}, {{parity}}, {{bits}}) {% endraw %}
       - value: |
-          # ExampleTestFunction asynPortIP name port value
-          ExampleTestFunction {{ PORT.IP }} {{ name }} {{ PORT }} {{ PORT.test_value }}
-          # PORT defaults to the id of PORT, i.e. PORT.name
-
-    databases:
-      - file: test.db
-        args:
-          name:
-          ip: "{{ PORT.IP }}"
-          value: "{{ PORT.test_value }}"
+          AsynIPConfigure({{name}}, {{port}}, {{stop}}, {{parity}}, {{bits}})
+          asynSetOption({{baud}}, 0, {{crtscts}}, {{disconnectOnReadTimeout}})
+          asynOctetSetInputEos({{input_eos}})
+          asynOctetSetOutputEos({{output_eos}})
```

### Comparing `ibek-2023.11.1b5/tests/samples/yaml/utils.ibek.support.yaml` & `ibek-3.4.0b2/tests/samples/support/utils.ibek.support.yaml`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/tests/sys-test.sh` & `ibek-3.4.0b2/tests/sys-test.sh`

 * *Files identical despite different names*

### Comparing `ibek-2023.11.1b5/tests/test_error.py` & `ibek-3.4.0b2/tests/test_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Tests to verify that the error handling works as expected.
 """
+
 from pathlib import Path
 
 import pytest
 from ruamel.yaml import YAML
 
 from ibek.ioc import clear_entity_model_ids, make_entity_models, make_ioc_model
 from ibek.support import Support
@@ -14,16 +15,16 @@
 
 def test_counter_reuse(tmp_path: Path, samples: Path):
     """
     Check you cannot redefine a counter with the same name and different params
     """
     UTILS.__reset__()
 
-    entity_file = samples / "yaml" / "bad_counter.ibek.ioc.yaml"
-    definition_file1 = samples / "yaml" / "utils.ibek.support.yaml"
+    entity_file = samples / "iocs" / "bad_counter.ibek.ioc.yaml"
+    definition_file1 = samples / "support" / "utils.ibek.support.yaml"
 
     with pytest.raises(ValueError) as ctx:
         run_cli("runtime", "generate", entity_file, definition_file1)
     assert (
         str(ctx.value)
         == "Redefining counter InterruptVector with different start/stop values"
     )
@@ -31,61 +32,61 @@
 
 def test_counter_overuse(tmp_path: Path, samples: Path):
     """
     Check that counter limits are enforced
     """
     UTILS.__reset__()
 
-    entity_file = samples / "yaml" / "bad_counter2.ibek.ioc.yaml"
-    definition_file1 = samples / "yaml" / "utils.ibek.support.yaml"
+    entity_file = samples / "iocs" / "bad_counter2.ibek.ioc.yaml"
+    definition_file1 = samples / "support" / "utils.ibek.support.yaml"
 
     with pytest.raises(ValueError) as ctx:
         run_cli("runtime", "generate", entity_file, definition_file1)
     assert str(ctx.value) == "Counter 195 exceeded stop value of 194"
 
 
 def test_bad_ref(tmp_path: Path, samples: Path):
     """
     Check bad object references are caught
     """
     UTILS.__reset__()
 
-    entity_file = samples / "yaml" / "bad_ref.ibek.ioc.yaml"
-    definition_file1 = samples / "yaml" / "objects.ibek.support.yaml"
-    definition_file2 = samples / "yaml" / "all.ibek.support.yaml"
+    entity_file = samples / "iocs" / "bad_ref.ibek.ioc.yaml"
+    definition_file1 = samples / "support" / "asyn.ibek.support.yaml"
+    definition_file2 = samples / "support" / "motorSim.ibek.support.yaml"
 
     with pytest.raises(ValueError) as ctx:
         run_cli("runtime", "generate", entity_file, definition_file1, definition_file2)
-    assert "object Ref2 not found" in str(ctx.value)
+    assert "object controllerOnePort_BAD_REF not found" in str(ctx.value)
 
 
 def test_bad_db(tmp_path: Path, samples: Path):
     """
     Check bad database args are caught
     """
     UTILS.__reset__()
 
-    entity_file = samples / "yaml" / "bad_db.ibek.ioc.yaml"
-    definition_file1 = samples / "yaml" / "bad_db.ibek.support.yaml"
+    entity_file = samples / "iocs" / "bad_db.ibek.ioc.yaml"
+    definition_file1 = samples / "support" / "bad_db.ibek.support.yaml"
 
     with pytest.raises(ValueError) as ctx:
         run_cli("runtime", "generate", entity_file, definition_file1)
     assert "'non-existant' in database template 'test.db' not found" in str(ctx.value)
 
 
 def test_loading_module_twice(tmp_path: Path, samples: Path):
     """
     Verify we get a sensible error if we try to load a module twice
     without clearing the entity model ids
     """
 
     clear_entity_model_ids()
 
-    definition_file = samples / "yaml" / "objects.ibek.support.yaml"
-    instance_file = samples / "yaml" / "objects.ibek.ioc.yaml"
+    definition_file = samples / "support" / "utils.ibek.support.yaml"
+    instance_file = samples / "iocs" / "utils.ibek.ioc.yaml"
 
     support = Support(**YAML(typ="safe").load(definition_file))
     entities1 = make_entity_models(support)
     entities2 = make_entity_models(support)
 
     generic_ioc1 = make_ioc_model(entities1)
     generic_ioc2 = make_ioc_model(entities2)
@@ -100,14 +101,14 @@
 
 def test_defaults(tmp_path: Path, samples: Path):
     """
     Check you cannot redefine a counter with the same name and different params
     """
 
     clear_entity_model_ids()
-    entity_file = samples / "yaml" / "bad_default.ibek.ioc.yaml"
-    definition_file1 = samples / "yaml" / "objects.ibek.support.yaml"
+    entity_file = samples / "iocs" / "bad_default.ibek.ioc.yaml"
+    definition_file1 = samples / "support" / "asyn.ibek.support.yaml"
 
     with pytest.raises(ValueError) as ctx:
         run_cli("runtime", "generate", entity_file, definition_file1)
 
     assert "Field required [type=missing" in str(ctx.value)
```

### Comparing `ibek-2023.11.1b5/tests/test_support.py` & `ibek-3.4.0b2/tests/test_support.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Unit tests for the support subcommand"""
+
 from pathlib import Path
 
 from ibek.support_cmds.files import symlink_files
 
 
 def test_symlink_ibek(tmp_path: Path, samples: Path):
-    symlink_files(samples / "yaml", "*.ibek.support.yaml", tmp_path)
+    symlink_files(samples / "support", "*.ibek.support.yaml", tmp_path)
 
     assert sorted([f.name for f in tmp_path.iterdir()]) == [
-        "all.ibek.support.yaml",
+        "asyn.ibek.support.yaml",
         "bad_db.ibek.support.yaml",
-        "objects.ibek.support.yaml",
+        "motorSim.ibek.support.yaml",
         "utils.ibek.support.yaml",
     ]
 
 
 def test_symlink_pvi(tmp_path: Path, samples: Path):
-    symlink_files(samples / "yaml", "*.pvi.device.yaml", tmp_path)
+    symlink_files(samples / "support", "*.pvi.device.yaml", tmp_path)
 
     assert [f.name for f in tmp_path.iterdir()] == ["simple.pvi.device.yaml"]
```

### Comparing `ibek-2023.11.1b5/tests/test_unit.py` & `ibek-3.4.0b2/tests/test_unit.py`

 * *Files identical despite different names*

