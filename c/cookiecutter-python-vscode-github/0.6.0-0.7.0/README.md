# Comparing `tmp/cookiecutter-python-vscode-github-0.6.0.tar.gz` & `tmp/cookiecutter_python_vscode_github-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter-python-vscode-github-0.6.0.tar", last modified: Sat Feb 10 16:12:54 2024, max compression
+gzip compressed data, was "cookiecutter_python_vscode_github-0.7.0.tar", last modified: Thu May  2 00:12:02 2024, max compression
```

## Comparing `cookiecutter-python-vscode-github-0.6.0.tar` & `cookiecutter_python_vscode_github-0.7.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:54.103684 cookiecutter-python-vscode-github-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:54.099684 cookiecutter-python-vscode-github-0.6.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/.devcontainer/bash.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/.devcontainer/devcontainer.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/.devcontainer/devcontainer.sh
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:54.091683 cookiecutter-python-vscode-github-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:54.099684 cookiecutter-python-vscode-github-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/.github/workflows/makefile.yml
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/.shellcheckrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:54.099684 cookiecutter-python-vscode-github-0.6.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-02-10 16:12:54.103684 cookiecutter-python-vscode-github-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:54.099684 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/cookiecutter.json
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-10 16:12:54.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:54.099684 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:54.103684 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.devcontainer/bash.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.devcontainer/devcontainer.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.devcontainer/devcontainer.sh
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:54.095684 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:54.103684 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.github/workflows/makefile.yml
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.shellcheckrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:54.103684 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/cookiecutter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/requirements-prod.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:54.103684 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/tests/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:54.103684 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug_underscore}}/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug_underscore}}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug_underscore}}/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:54.103684 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-02-10 16:12:54.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-02-10 16:12:54.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 16:12:54.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-10 16:12:54.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-10 16:12:54.000000 cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    55830 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/requirements-dev.lock
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/requirements-prod.lock
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/requirements-prod.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-10 16:12:54.103684 cookiecutter-python-vscode-github-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:54.103684 cookiecutter-python-vscode-github-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-02-10 16:12:44.000000 cookiecutter-python-vscode-github-0.6.0/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:02.587546 cookiecutter_python_vscode_github-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:02.579546 cookiecutter_python_vscode_github-0.7.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/.devcontainer/bash.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/.devcontainer/devcontainer.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/.devcontainer/devcontainer.sh
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:02.575546 cookiecutter_python_vscode_github-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:02.579546 cookiecutter_python_vscode_github-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/.github/workflows/makefile.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/.shellcheckrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:02.579546 cookiecutter_python_vscode_github-0.7.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-02 00:12:02.587546 cookiecutter_python_vscode_github-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:02.579546 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/cookiecutter.json
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 00:12:02.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:02.583546 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:02.583546 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.devcontainer/bash.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.devcontainer/devcontainer.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.devcontainer/devcontainer.sh
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:02.575546 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:02.583546 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.github/workflows/makefile.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.shellcheckrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:02.583546 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/cookiecutter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/requirements-prod.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:02.583546 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:02.587546 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug_underscore}}/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug_underscore}}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug_underscore}}/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:02.587546 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-02 00:12:02.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-02 00:12:02.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:12:02.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-02 00:12:02.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 00:12:02.000000 cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    56414 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/requirements-dev.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/requirements-prod.lock
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/requirements-prod.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 00:12:02.587546 cookiecutter_python_vscode_github-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:02.587546 cookiecutter_python_vscode_github-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-02 00:11:57.000000 cookiecutter_python_vscode_github-0.7.0/tests/test_main.py
```

### Comparing `cookiecutter-python-vscode-github-0.6.0/.devcontainer/devcontainer.dockerfile` & `cookiecutter_python_vscode_github-0.7.0/.devcontainer/devcontainer.dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM python:3.11.7-bookworm
+FROM python:3.11.9-bookworm
 
 # Set the default shell to bash instead of sh
 ENV SHELL /bin/bash
 
 # Install Linux tools
 RUN apt-get update -q && \
     DEBIAN_FRONTEND=noninteractive apt-get install -yq --no-install-recommends \
```

### Comparing `cookiecutter-python-vscode-github-0.6.0/.devcontainer/devcontainer.json` & `cookiecutter_python_vscode_github-0.7.0/.devcontainer/devcontainer.json`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,18 @@
   "name": "cookiecutter-python-vscode-github",
   // Use docker while docker-compose doesn't support --gpus
   "dockerFile": "devcontainer.dockerfile",
   "context": "..",
   "workspaceMount": "type=bind,source=${localWorkspaceFolder},target=/workspace/cookiecutter-python-vscode-github",
   "workspaceFolder": "/workspace/cookiecutter-python-vscode-github",
   "mounts": [
-    "type=bind,source=${localEnv:HOME}${localEnv:USERPROFILE}/.ssh,target=/home/user/.ssh",
-    "type=bind,source=${localEnv:HOME}${localEnv:USERPROFILE}/.gitconfig,target=/home/user/.gitconfig",
     "type=volume,source=cookiecutter-python-vscode-github_vscode-server,target=/home/user/.vscode-server",
     "type=volume,source=home-cache,target=/home/user/.cache"
   ],
-  "postCreateCommand": "make devenv",
+  "postCreateCommand": "make env",
   "customizations": {
     "vscode": {
       "extensions": [
         "ms-python.python",
         "VisualStudioExptTeam.vscodeintellicode",
         "GitHub.vscode-pull-request-github",
         "github.vscode-github-actions",
```

### Comparing `cookiecutter-python-vscode-github-0.6.0/.github/workflows/python-publish.yml` & `cookiecutter_python_vscode_github-0.7.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cookiecutter-python-vscode-github-0.6.0/.gitignore` & `cookiecutter_python_vscode_github-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cookiecutter-python-vscode-github-0.6.0/.pylintrc` & `cookiecutter_python_vscode_github-0.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `cookiecutter-python-vscode-github-0.6.0/LICENSE` & `cookiecutter_python_vscode_github-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cookiecutter-python-vscode-github-0.6.0/Makefile` & `cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/Makefile`

 * *Files 18% similar despite different names*

```diff
@@ -1,145 +1,190 @@
+SHELL:=/bin/bash
 PRETTIER_DIFF=$(shell prettier . --list-different)
-GIT_FILES=git ls-files -z | tr '\0' '\n'
-GIT_UNTRACKED_FILES=git ls-files -z --exclude-standard --others | tr '\0' '\n'
-# If there is no deleted file, "grep --invert-match" is deactivated by the NULL string returned by "echo -e '\0'",
+GIT_FILES=git ls-files
+GIT_UNTRACKED_FILES=git ls-files --exclude-standard --others
+# If there is no deleted file, "grep --invert-match" is deactivated by the string returned by "echo -e '//'",
 #    otherwise, "grep --invert-match" uses the list of deleted files.
-GREP_NOT_DELETED=grep --invert-match "$$( ( [ -z "$$(git ls-files --deleted)" ] && echo -e '\0' ) || ( git ls-files -z --deleted | tr '\0' '\n' ) )"
-GREP_PACKAGE=grep '^cookiecutter_python_vscode_github/'
+GREP_NOT_DELETED=grep --invert-match "$$( ( [ -z "$$(git ls-files --deleted)" ] && echo -e '//' ) || ( git ls-files --deleted ) )"
+GREP_PACKAGE=grep '^{{cookiecutter.project_slug_underscore}}/'
 GREP_TESTS=grep '^tests/'
 GREP_PYTHON=grep '\.py$$'
 GREP_NOT_PYTHON=grep --invert-match '\.py$$'
 GREP_SHELL=grep '\.sh$$'
+GREP_NOT_TEMPLATE=grep --invert-match '{% raw %}{{cookiecutter.project_slug}}{% endraw %}/'
 PACKAGE_SRC=$(shell ${GIT_FILES} | ${GREP_PACKAGE} | ${GREP_PYTHON} | ${GREP_NOT_DELETED}) $(shell ${GIT_UNTRACKED_FILES} | ${GREP_PACKAGE} | ${GREP_PYTHON})
 PACKAGE_DATA=$(shell ${GIT_FILES} | ${GREP_PACKAGE} | ${GREP_NOT_PYTHON} | ${GREP_NOT_DELETED}) $(shell ${GIT_UNTRACKED_FILES} | ${GREP_PACKAGE} | ${GREP_NOT_PYTHON})
 TESTS_SRC=$(shell ${GIT_FILES} | ${GREP_TESTS} | ${GREP_PYTHON} | ${GREP_NOT_DELETED}) $(shell ${GIT_UNTRACKED_FILES} | ${GREP_TESTS} | ${GREP_PYTHON})
 TESTS_DATA=$(shell ${GIT_FILES} | ${GREP_TESTS} | ${GREP_NOT_PYTHON} | ${GREP_NOT_DELETED}) $(shell ${GIT_UNTRACKED_FILES} | ${GREP_TESTS} | ${GREP_NOT_PYTHON})
+MYPY_SRC=$(shell ${GIT_FILES} | ${GREP_NOT_TEMPLATE} | ${GREP_PYTHON} | ${GREP_NOT_DELETED}) $(shell ${GIT_UNTRACKED_FILES} | ${GREP_NOT_TEMPLATE} | ${GREP_PYTHON})
 SHELL_SRC=$(shell ${GIT_FILES} | ${GREP_SHELL} | ${GREP_NOT_DELETED}) $(shell ${GIT_UNTRACKED_FILES} | ${GREP_SHELL})
 VENV_BIN=.venv/bin/
 PYTHON=$(shell env --ignore-environment which python)
+PIP_TOOLS_VERSION=$(shell cat requirements-dev.lock 2>/dev/null | grep '^pip-tools==' | grep --extended-regexp --only-matching '==[.0-9]+')
+SKIP=[ $$(stat -c %Y $|) -gt $$(stat -c %Y $@ 2> /dev/null || echo 0) ] || 
+GIT_STATUS=git status --porcelain
+DONE=@echo $@ done.
 TOUCH=@mkdir --parents .cache/make && date > $@
 
 ## devcontainer: Create devcontainer.
 .PHONY: devcontainer
 devcontainer:
 	bash .devcontainer/devcontainer.sh
 
-## devenv      : Setup development environment (.bashrc, .bash_aliases and pre-commit hooks).
-.PHONY: devenv
-devenv: .cache/make/sync
+## env      : Setup environment (.bashrc, .bash_aliases and pre-commit hooks).
+~/.bash_aliases: .devcontainer/bash.sh
 	bash .devcontainer/bash.sh
+.git/hooks/pre-commit: .cache/make/install .pre-commit-config.yaml
 	${VENV_BIN}pre-commit install --overwrite --hook-type=pre-commit --hook-type=pre-push
+.PHONY: env
+env: ~/.bash_aliases .git/hooks/pre-commit
 
 ## clean       : Delete caches and files generated during the build.
 clean:
-	rm -rf .venv .cache/make cookiecutter-python-vscode-github.egg-info .pytest_cache tests/.pytest_cache dist requirements-dev-*.txt
+	rm -rf .venv .cache/make {{cookiecutter.project_slug}}.egg-info .pytest_cache tests/.pytest_cache dist requirements-dev-*.txt
 
 ## main        : Run all necessary rules to build the Python package (default).
 .DEFAULT_GOAL:=main
-main: venv install lock sync format secure lint test package smoke
+main: venv lock install format secure lint test package smoke
 .PHONY: main
 
 ## venv        : Create virtual environemnt.
-${VENV_BIN}activate: ${PYTHON} Makefile .devcontainer/devcontainer.dockerfile
+${VENV_BIN}activate: Makefile .devcontainer/devcontainer.dockerfile
 	${PYTHON} -m venv --clear --prompt='cookiecutter-python-vscode-github' .venv
 .PHONY: venv
 venv: ${VENV_BIN}activate
-
-## install     : Install most recent versions of the development dependencies.
-.cache/make/install: ${VENV_BIN}activate pyproject.toml requirements-dev.txt constraints.txt
-	${VENV_BIN}pip install --quiet --requirement=requirements-dev.txt --editable=. --constraint=constraints.txt
-	${TOUCH}
-.PHONY: install
-install: .cache/make/install
+	${DONE}
 
 ## lock        : Lock development and production dependencies.
-requirements-dev.lock: .cache/make/install requirements-dev.txt constraints.txt pyproject.toml requirements-prod.txt
+${VENV_BIN}pip-compile: ${VENV_BIN}activate
+	${VENV_BIN}pip install --quiet --disable-pip-version-check pip-tools${PIP_TOOLS_VERSION}
+requirements-dev.lock: ${VENV_BIN}pip-compile requirements-dev.txt constraints.txt pyproject.toml requirements-prod.txt
 	${VENV_BIN}pip-compile --quiet --resolver=backtracking --generate-hashes --strip-extras --allow-unsafe --output-file=requirements-dev.lock --no-header --no-annotate requirements-dev.txt pyproject.toml --constraint=constraints.txt
 requirements-prod.lock: pyproject.toml requirements-prod.txt requirements-dev.lock
 	${VENV_BIN}pip-compile --quiet --resolver=backtracking --generate-hashes --strip-extras --allow-unsafe --output-file=requirements-prod.lock --no-header --no-annotate pyproject.toml --constraint=requirements-dev.lock
 .PHONY: lock
 lock: requirements-dev.lock requirements-prod.lock
+	${DONE}
 
 ## unlock      : Unlock development and production dependencies.
 .PHONY: unlock
 unlock:
 	rm -rf requirements-*.lock
 
-## sync        : Syncronize development dependencies in the environment according to requirements-dev.lock.
-.cache/make/sync: pyproject.toml requirements-dev.lock
-	${VENV_BIN}pip-sync --quiet requirements-dev.lock
-	${VENV_BIN}pip install --quiet --editable=.
+## install     : Install development dependencies according to requirements-dev.lock.
+.cache/make/install: pyproject.toml requirements-dev.lock
+	${VENV_BIN}pip-sync --quiet --pip-args="--disable-pip-version-check" requirements-dev.lock
+	${VENV_BIN}pip install --quiet --disable-pip-version-check --editable=.
 	${TOUCH}
-.PHONY: sync
-sync: .cache/make/sync
+.PHONY: install
+install: .cache/make/install
+	${DONE}
 
 ## format      : Format source code.
 # If docformatter fails, the script ignores exit status 3, because that code is returned when docformatter changes any file.
 # If the variable PRETTIER_DIFF is not empty, prettier is executed. Ignore errors because prettier is not available in GitHub Actions.
-.cache/make/format: .cache/make/sync ${PRETTIER_DIFF} ${PACKAGE_SRC} ${TESTS_SRC}
+.cache/make/format-all: .cache/make/install
 	${VENV_BIN}pyupgrade --py311-plus --exit-zero-even-if-changed ${PACKAGE_SRC} ${TESTS_SRC}
-	${VENV_BIN}isort --profile black cookiecutter_python_vscode_github tests
-	${VENV_BIN}black cookiecutter_python_vscode_github tests
-	${VENV_BIN}docformatter --in-place --recursive cookiecutter_python_vscode_github tests || [ "$$?" -eq "3" ]
-	-[ -z "${PRETTIER_DIFF}" ] || prettier ${PRETTIER_DIFF} --write
+	${VENV_BIN}isort --profile black ${PACKAGE_SRC} ${TESTS_SRC}
+	${VENV_BIN}black --quiet ${PACKAGE_SRC} ${TESTS_SRC}
+	${VENV_BIN}docformatter --in-place ${PACKAGE_SRC} ${TESTS_SRC} || [ "$$?" -eq "3" ]
+	[ -z "${PRETTIER_DIFF}" ] || prettier ${PRETTIER_DIFF} --write
+	${TOUCH}
+.cache/make/format-change: ${PACKAGE_SRC} ${TESTS_SRC} | .cache/make/format-all
+	${SKIP}${VENV_BIN}pyupgrade --py311-plus --exit-zero-even-if-changed $?
+	${SKIP}${VENV_BIN}isort --profile black $?
+	${SKIP}${VENV_BIN}black --quiet $?
+	${SKIP}${VENV_BIN}docformatter --in-place $? || [ "$$?" -eq "3" ]
+	${TOUCH}
+.cache/make/prettier-change: ${PRETTIER_DIFF} | .cache/make/format-all
+	${SKIP}[ -z "$?" ] || prettier $? --write
+	${TOUCH}
+.cache/make/format: .cache/make/format-all .cache/make/format-change .cache/make/prettier-change
 	${TOUCH}
 .PHONY: format
 format: .cache/make/format
+	${DONE}
 
 ## secure      : Run vulnerability scanners on source code and production dependencies.
-.cache/make/pip-audit: .cache/make/sync requirements-prod.lock
+.cache/make/pip-audit: .cache/make/install requirements-prod.lock
 	${VENV_BIN}pip-audit --cache-dir=${HOME}/.cache/pip-audit --requirement=requirements-prod.lock
 	${TOUCH}
-.cache/make/bandit: .cache/make/format ${PACKAGE_SRC}
-	${VENV_BIN}bandit --recursive cookiecutter_python_vscode_github
+.cache/make/bandit-all: .cache/make/install | .cache/make/format
+	${VENV_BIN}bandit --quiet ${PACKAGE_SRC}
+	${TOUCH}
+.cache/make/bandit-change: ${PACKAGE_SRC} | .cache/make/bandit-all
+	${SKIP}${VENV_BIN}bandit --quiet $?
 	${TOUCH}
 .PHONY: secure
-secure: .cache/make/pip-audit .cache/make/bandit
+secure: .cache/make/pip-audit .cache/make/bandit-all .cache/make/bandit-change
+	${DONE}
 
 ## lint        : Run static code analysers on source code.
-.cache/make/lint: .cache/make/format ${PACKAGE_SRC} ${TESTS_SRC} ${SHELL_SRC} .pylintrc mypy.ini .shellcheckrc
-	${VENV_BIN}pylint cookiecutter_python_vscode_github
-	${VENV_BIN}mypy cookiecutter_python_vscode_github tests
+.cache/make/lint-all: .cache/make/install .pylintrc mypy.ini .shellcheckrc | .cache/make/format
+	${VENV_BIN}pylint --errors-only ${PACKAGE_SRC}
+	${VENV_BIN}mypy ${MYPY_SRC}
 	shellcheck ${SHELL_SRC}
 	${TOUCH}
+.cache/make/pylint-change: ${PACKAGE_SRC} | .cache/make/lint-all
+	${SKIP}${VENV_BIN}pylint --errors-only $?
+	${TOUCH}
+.cache/make/mypy-change: ${MYPY_SRC} | .cache/make/lint-all
+	${SKIP}${VENV_BIN}mypy $?
+	${TOUCH}
+.cache/make/shellcheck-change: ${SHELL_SRC} | .cache/make/lint-all
+	${SKIP}shellcheck $?
+	${TOUCH}
+.cache/make/lint: .cache/make/lint-all .cache/make/pylint-change .cache/make/mypy-change .cache/make/shellcheck-change
+	${TOUCH}
 .PHONY: lint
 lint: .cache/make/lint
+	${DONE}
 
 ## test        : Run automated tests.
 .cache/make/test: .cache/make/format ${PACKAGE_SRC} ${PACKAGE_DATA} ${TESTS_SRC} ${TESTS_DATA}
-	${VENV_BIN}pytest --cov=cookiecutter_python_vscode_github --cov-report=term-missing tests
+	${VENV_BIN}pytest --cov={{cookiecutter.project_slug_underscore}} --cov-report=term-missing tests
 	${TOUCH}
 .PHONY: test
 test: .cache/make/test
+	${DONE}
 	
 ## package     : Create wheel.
 .cache/make/package: .cache/make/format ${PACKAGE_SRC} ${PACKAGE_DATA} pyproject.toml
 	rm -rf dist/
-	${VENV_BIN}python -m build
+	${VENV_BIN}python -m build --wheel
 	${TOUCH}
 .PHONY: package
 package: .cache/make/package
+	${DONE}
 
 ## smoke       : Smoke test wheel.
 .cache/make/smoke: .cache/make/package
-	${VENV_BIN}pip install --quiet dist/*.whl
-	${VENV_BIN}cookiecutter-python-vscode-github --help
-	${VENV_BIN}cookiecutter-python-vscode-github --version
-	${VENV_BIN}pip install --quiet --editable=.
+	${VENV_BIN}pip install --quiet --disable-pip-version-check dist/*.whl
+	${VENV_BIN}{{cookiecutter.project_slug}} --help
+	${VENV_BIN}{{cookiecutter.project_slug}} --version
+	${VENV_BIN}pip install --quiet --disable-pip-version-check --editable=.
 	${TOUCH}
 .PHONY: smoke
 smoke: .cache/make/smoke
+	${DONE}
+
+## check       : Check if there are pending changes in the working tree.
+.PHONY: check
+check:
+	${GIT_STATUS}
+	[ -z "$$(${GIT_STATUS})" ]
+	${DONE}
 
 ## testpypi    : Upload Python package to https://test.pypi.org/.
 .PHONY: testpypi
-testpypi: .cache/make/sync
+testpypi: .cache/make/package
 	${VENV_BIN}twine upload --repository testpypi dist/*.whl
 
 ## cookie      : Update project using cookiecutter-python-vscode-github template.
 .PHONY: cookie
-cookie: .cache/make/sync
+cookie: .cache/make/install
 	${VENV_BIN}cookiecutter --overwrite-if-exists --output-dir=.. --no-input --config-file=cookiecutter.yaml $$(cookiecutter-python-vscode-github)
 
 ## help        : Show this help message.
 .PHONY: help
 help:
 	@sed -n 's/^##//p' Makefile
```

### Comparing `cookiecutter-python-vscode-github-0.6.0/PKG-INFO` & `cookiecutter_python_vscode_github-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiecutter-python-vscode-github
-Version: 0.6.0
+Version: 0.7.0
 Summary: Cookiecutter Python VSCode GitHub provides a Python Package template with an IDE (Visual Studio Code) and a CI/CD (GitHub Actions) already setup.
 Author-email: "Dinaldo A. Pessoa" <dinaldoap@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 dinaldoap
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cookiecutter-python-vscode-github-0.6.0/cookiecutter.yaml` & `cookiecutter_python_vscode_github-0.7.0/cookiecutter.yaml`

 * *Files identical despite different names*

### Comparing `cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/__main__.py` & `cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/__main__.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/cookiecutter.json` & `cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.devcontainer/devcontainer.dockerfile` & `cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.devcontainer/devcontainer.dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM python:3.11.7-bookworm
+FROM python:3.11.9-bookworm
 
 # Set the default shell to bash instead of sh
 ENV SHELL /bin/bash
 
 # Install Linux tools
 RUN apt-get update -q && \
     DEBIAN_FRONTEND=noninteractive apt-get install -yq --no-install-recommends \
```

### Comparing `cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.devcontainer/devcontainer.json` & `cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.devcontainer/devcontainer.json`

 * *Files 11% similar despite different names*

```diff
@@ -2,20 +2,18 @@
   "name": "{{cookiecutter.project_slug}}",
   // Use docker while docker-compose doesn't support --gpus
   "dockerFile": "devcontainer.dockerfile",
   "context": "..",
   "workspaceMount": "type=bind,source=${localWorkspaceFolder},target=/workspace/{{cookiecutter.project_slug}}",
   "workspaceFolder": "/workspace/{{cookiecutter.project_slug}}",
   "mounts": [
-    "type=bind,source=${localEnv:HOME}${localEnv:USERPROFILE}/.ssh,target=/home/user/.ssh",
-    "type=bind,source=${localEnv:HOME}${localEnv:USERPROFILE}/.gitconfig,target=/home/user/.gitconfig",
     "type=volume,source={{cookiecutter.project_slug}}_vscode-server,target=/home/user/.vscode-server",
     "type=volume,source=home-cache,target=/home/user/.cache"
   ],
-  "postCreateCommand": "make devenv",
+  "postCreateCommand": "make env",
   "customizations": {
     "vscode": {
       "extensions": [
         "ms-python.python",
         "VisualStudioExptTeam.vscodeintellicode",
         "GitHub.vscode-pull-request-github",
         "github.vscode-github-actions",
```

### Comparing `cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.github/workflows/python-publish.yml` & `cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.gitignore` & `cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.pylintrc` & `cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/.pylintrc`

 * *Files identical despite different names*

### Comparing `cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/cookiecutter.yaml` & `cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/cookiecutter.yaml`

 * *Files identical despite different names*

### Comparing `cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/pyproject.toml` & `cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github/{{cookiecutter.project_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github.egg-info/PKG-INFO` & `cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiecutter-python-vscode-github
-Version: 0.6.0
+Version: 0.7.0
 Summary: Cookiecutter Python VSCode GitHub provides a Python Package template with an IDE (Visual Studio Code) and a CI/CD (GitHub Actions) already setup.
 Author-email: "Dinaldo A. Pessoa" <dinaldoap@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 dinaldoap
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cookiecutter-python-vscode-github-0.6.0/cookiecutter_python_vscode_github.egg-info/SOURCES.txt` & `cookiecutter_python_vscode_github-0.7.0/cookiecutter_python_vscode_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cookiecutter-python-vscode-github-0.6.0/pyproject.toml` & `cookiecutter_python_vscode_github-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cookiecutter-python-vscode-github-0.6.0/requirements-dev.lock` & `cookiecutter_python_vscode_github-0.7.0/requirements-dev.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 arrow==1.3.0 \
     --hash=sha256:c728b120ebc00eb84e01882a6f5e7927a53960aa990ce7dd2b10f39005a67f80 \
     --hash=sha256:d4540617648cb5f895730f1ad8c82a65f2dad0166f57b75f3ca54759c4d67a85
-astroid==3.0.2 \
-    --hash=sha256:4a61cf0a59097c7bb52689b0fd63717cd2a8a14dc9f1eee97b82d814881c8c91 \
-    --hash=sha256:d6e62862355f60e716164082d6b4b041d38e2a8cf1c7cd953ded5108bac8ff5c
-bandit==1.7.7 \
-    --hash=sha256:17e60786a7ea3c9ec84569fd5aee09936d116cb0cb43151023258340dbffb7ed \
-    --hash=sha256:527906bec6088cb499aae31bc962864b4e77569e9d529ee51df3a93b4b8ab28a
+astroid==3.1.0 \
+    --hash=sha256:951798f922990137ac090c53af473db7ab4e70c770e6d7fae0cec59f74411819 \
+    --hash=sha256:ac248253bfa4bd924a0de213707e7ebeeb3138abeb48d798784ead1e56d419d4
+backports-tarfile==1.0.0 \
+    --hash=sha256:2688f159c21afd56a07b75f01306f9f52c79aebcc5f4a117fb8fbb4445352c75 \
+    --hash=sha256:bcd36290d9684beb524d3fe74f4a2db056824c47746583f090b8e55daf0776e4
+bandit==1.7.8 \
+    --hash=sha256:36de50f720856ab24a24dbaa5fee2c66050ed97c1477e0a1159deab1775eab6b \
+    --hash=sha256:509f7af645bc0cd8fd4587abc1a038fc795636671ee8204d502b933aee44f381
 binaryornot==0.4.4 \
     --hash=sha256:359501dfc9d40632edc9fac890e19542db1a287bbcfa58175b66658392018061 \
     --hash=sha256:b8b71173c917bddcd2c16070412e369c3ed7f0528926f70cac18a6c97fd563e4
-black==24.1.1 \
-    --hash=sha256:0269dfdea12442022e88043d2910429bed717b2d04523867a85dacce535916b8 \
-    --hash=sha256:07204d078e25327aad9ed2c64790d681238686bce254c910de640c7cc4fc3aa6 \
-    --hash=sha256:08b34e85170d368c37ca7bf81cf67ac863c9d1963b2c1780c39102187ec8dd62 \
-    --hash=sha256:1a95915c98d6e32ca43809d46d932e2abc5f1f7d582ffbe65a5b4d1588af7445 \
-    --hash=sha256:2588021038bd5ada078de606f2a804cadd0a3cc6a79cb3e9bb3a8bf581325a4c \
-    --hash=sha256:2fa6a0e965779c8f2afb286f9ef798df770ba2b6cee063c650b96adec22c056a \
-    --hash=sha256:34afe9da5056aa123b8bfda1664bfe6fb4e9c6f311d8e4a6eb089da9a9173bf9 \
-    --hash=sha256:3897ae5a21ca132efa219c029cce5e6bfc9c3d34ed7e892113d199c0b1b444a2 \
-    --hash=sha256:40657e1b78212d582a0edecafef133cf1dd02e6677f539b669db4746150d38f6 \
-    --hash=sha256:48b5760dcbfe5cf97fd4fba23946681f3a81514c6ab8a45b50da67ac8fbc6c7b \
-    --hash=sha256:5242ecd9e990aeb995b6d03dc3b2d112d4a78f2083e5a8e86d566340ae80fec4 \
-    --hash=sha256:5cdc2e2195212208fbcae579b931407c1fa9997584f0a415421748aeafff1168 \
-    --hash=sha256:5d7b06ea8816cbd4becfe5f70accae953c53c0e53aa98730ceccb0395520ee5d \
-    --hash=sha256:7258c27115c1e3b5de9ac6c4f9957e3ee2c02c0b39222a24dc7aa03ba0e986f5 \
-    --hash=sha256:854c06fb86fd854140f37fb24dbf10621f5dab9e3b0c29a690ba595e3d543024 \
-    --hash=sha256:a21725862d0e855ae05da1dd25e3825ed712eaaccef6b03017fe0853a01aa45e \
-    --hash=sha256:a83fe522d9698d8f9a101b860b1ee154c1d25f8a82ceb807d319f085b2627c5b \
-    --hash=sha256:b3d64db762eae4a5ce04b6e3dd745dcca0fb9560eb931a5be97472e38652a161 \
-    --hash=sha256:e298d588744efda02379521a19639ebcd314fba7a49be22136204d7ed1782717 \
-    --hash=sha256:e2c8dfa14677f90d976f68e0c923947ae68fa3961d61ee30976c388adc0b02c8 \
-    --hash=sha256:ecba2a15dfb2d97105be74bbfe5128bc5e9fa8477d8c46766505c1dda5883aac \
-    --hash=sha256:fc1ec9aa6f4d98d022101e015261c056ddebe3da6a8ccfc2c792cbe0349d48b7
+black==24.3.0 \
+    --hash=sha256:2818cf72dfd5d289e48f37ccfa08b460bf469e67fb7c4abb07edc2e9f16fb63f \
+    --hash=sha256:41622020d7120e01d377f74249e677039d20e6344ff5851de8a10f11f513bf93 \
+    --hash=sha256:4acf672def7eb1725f41f38bf6bf425c8237248bb0804faa3965c036f7672d11 \
+    --hash=sha256:4be5bb28e090456adfc1255e03967fb67ca846a03be7aadf6249096100ee32d0 \
+    --hash=sha256:4f1373a7808a8f135b774039f61d59e4be7eb56b2513d3d2f02a8b9365b8a8a9 \
+    --hash=sha256:56f52cfbd3dabe2798d76dbdd299faa046a901041faf2cf33288bc4e6dae57b5 \
+    --hash=sha256:65b76c275e4c1c5ce6e9870911384bff5ca31ab63d19c76811cb1fb162678213 \
+    --hash=sha256:65c02e4ea2ae09d16314d30912a58ada9a5c4fdfedf9512d23326128ac08ac3d \
+    --hash=sha256:6905238a754ceb7788a73f02b45637d820b2f5478b20fec82ea865e4f5d4d9f7 \
+    --hash=sha256:79dcf34b33e38ed1b17434693763301d7ccbd1c5860674a8f871bd15139e7837 \
+    --hash=sha256:7bb041dca0d784697af4646d3b62ba4a6b028276ae878e53f6b4f74ddd6db99f \
+    --hash=sha256:7d5e026f8da0322b5662fa7a8e752b3fa2dac1c1cbc213c3d7ff9bdd0ab12395 \
+    --hash=sha256:9f50ea1132e2189d8dff0115ab75b65590a3e97de1e143795adb4ce317934995 \
+    --hash=sha256:a0c9c4a0771afc6919578cec71ce82a3e31e054904e7197deacbc9382671c41f \
+    --hash=sha256:aadf7a02d947936ee418777e0247ea114f78aff0d0959461057cae8a04f20597 \
+    --hash=sha256:b5991d523eee14756f3c8d5df5231550ae8993e2286b8014e2fdea7156ed0959 \
+    --hash=sha256:bf21b7b230718a5f08bd32d5e4f1db7fc8788345c8aea1d155fc17852b3410f5 \
+    --hash=sha256:c45f8dff244b3c431b36e3224b6be4a127c6aca780853574c00faf99258041eb \
+    --hash=sha256:c7ed6668cbbfcd231fa0dc1b137d3e40c04c7f786e626b405c62bcd5db5857e4 \
+    --hash=sha256:d7de8d330763c66663661a1ffd432274a2f92f07feeddd89ffd085b5744f85e7 \
+    --hash=sha256:e19cb1c6365fd6dc38a6eae2dcb691d7d83935c10215aef8e6c38edee3f77abd \
+    --hash=sha256:e2af80566f43c85f5797365077fb64a393861a3730bd110971ab7a0c94e873e7
 boolean-py==4.0 \
     --hash=sha256:17b9a181630e43dde1851d42bef546d616d5d9b4480357514597e78b203d06e4 \
     --hash=sha256:2876f2051d7d6394a531d82dc6eb407faa0b01a0a0b3083817ccd7323b8d96bd
-build==1.0.3 \
-    --hash=sha256:538aab1b64f9828977f84bc63ae570b060a8ed1be419e7870b8b4fc5e6ea553b \
-    --hash=sha256:589bf99a67df7c9cf07ec0ac0e5e2ea5d4b37ac63301c4986d1acb126aa83f8f
-cachecontrol==0.13.1 \
-    --hash=sha256:95dedbec849f46dda3137866dc28b9d133fc9af55f5b805ab1291833e4457aa4 \
-    --hash=sha256:f012366b79d2243a6118309ce73151bf52a38d4a5dac8ea57f09bd29087e506b
-certifi==2023.11.17 \
-    --hash=sha256:9b469f3a900bf28dc19b8cfbf8019bf47f7fdd1a65a1d4ffb98fc14166beb4d1 \
-    --hash=sha256:e036ab49d5b79556f99cfc2d9320b34cfbe5be05c5871b51de9329f0603b0474
+build==1.2.1 \
+    --hash=sha256:526263f4870c26f26c433545579475377b2b7588b6f1eac76a001e873ae3e19d \
+    --hash=sha256:75e10f767a433d9a86e50d83f418e83efc18ede923ee5ff7df93b6cb0306c5d4
+cachecontrol==0.14.0 \
+    --hash=sha256:7db1195b41c81f8274a7bbd97c956f44e8348265a1bc7641c37dfebc39f0c938 \
+    --hash=sha256:f5bf3f0620c38db2e5122c0726bdebb0d16869de966ea6a2befe92470b740ea0
+certifi==2024.2.2 \
+    --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
+    --hash=sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1
 cffi==1.16.0 \
     --hash=sha256:0c9ef6ff37e974b73c25eecc13952c55bceed9112be2d9d938ded8e856138bcc \
     --hash=sha256:131fd094d1065b19540c3d72594260f118b231090295d8c34e19a7bbcf2e860a \
     --hash=sha256:1b8ebc27c014c59692bb2664c7d13ce7a6e9a629be20e54e7271fa696ff2b417 \
     --hash=sha256:2c56b361916f390cd758a57f2e16233eb4f64bcbeee88a4881ea90fca14dc6ab \
     --hash=sha256:2d92b25dbf6cae33f65005baf472d2c245c050b1ce709cc4588cdcdd5495b520 \
     --hash=sha256:31d13b0f99e0836b7ff893d37af07366ebc90b678b6664c955b54561fc36ef36 \
@@ -194,425 +197,431 @@
     --hash=sha256:f30c3cb33b24454a82faecaf01b19c18562b1e89558fb6c56de4d9118a032fd5 \
     --hash=sha256:fb69256e180cb6c8a894fee62b3afebae785babc1ee98b81cdf68bbca1987f33 \
     --hash=sha256:fd1abc0d89e30cc4e02e4064dc67fcc51bd941eb395c502aac3ec19fab46b519 \
     --hash=sha256:ff8fa367d09b717b2a17a052544193ad76cd49979c805768879cb63d9ca50561
 click==8.1.7 \
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
-cookiecutter==2.5.0 \
-    --hash=sha256:8aa2f12ed11bc05628651e9dc4353a10571dd9908aaaaeec959a2b9ea465a5d2 \
-    --hash=sha256:e61e9034748e3f41b8bd2c11f00d030784b48711c4d5c42363c50989a65331ec
-cookiecutter-python-vscode-github==0.5.0 \
-    --hash=sha256:3842ebb1fa006160539805137f5b39359a2217ee65d15b5fa100f160316c5be5 \
-    --hash=sha256:d30305eca0132feb7ec8e77dc000f4fa03ae7ecadf99972943164168bcb9d368
-coverage==7.4.1 \
-    --hash=sha256:0193657651f5399d433c92f8ae264aff31fc1d066deee4b831549526433f3f61 \
-    --hash=sha256:02f2edb575d62172aa28fe00efe821ae31f25dc3d589055b3fb64d51e52e4ab1 \
-    --hash=sha256:0491275c3b9971cdbd28a4595c2cb5838f08036bca31765bad5e17edf900b2c7 \
-    --hash=sha256:077d366e724f24fc02dbfe9d946534357fda71af9764ff99d73c3c596001bbd7 \
-    --hash=sha256:10e88e7f41e6197ea0429ae18f21ff521d4f4490aa33048f6c6f94c6045a6a75 \
-    --hash=sha256:18e961aa13b6d47f758cc5879383d27b5b3f3dcd9ce8cdbfdc2571fe86feb4dd \
-    --hash=sha256:1a78b656a4d12b0490ca72651fe4d9f5e07e3c6461063a9b6265ee45eb2bdd35 \
-    --hash=sha256:1ed4b95480952b1a26d863e546fa5094564aa0065e1e5f0d4d0041f293251d04 \
-    --hash=sha256:23b27b8a698e749b61809fb637eb98ebf0e505710ec46a8aa6f1be7dc0dc43a6 \
-    --hash=sha256:23f5881362dcb0e1a92b84b3c2809bdc90db892332daab81ad8f642d8ed55042 \
-    --hash=sha256:32a8d985462e37cfdab611a6f95b09d7c091d07668fdc26e47a725ee575fe166 \
-    --hash=sha256:3468cc8720402af37b6c6e7e2a9cdb9f6c16c728638a2ebc768ba1ef6f26c3a1 \
-    --hash=sha256:379d4c7abad5afbe9d88cc31ea8ca262296480a86af945b08214eb1a556a3e4d \
-    --hash=sha256:3cacfaefe6089d477264001f90f55b7881ba615953414999c46cc9713ff93c8c \
-    --hash=sha256:3e3424c554391dc9ef4a92ad28665756566a28fecf47308f91841f6c49288e66 \
-    --hash=sha256:46342fed0fff72efcda77040b14728049200cbba1279e0bf1188f1f2078c1d70 \
-    --hash=sha256:536d609c6963c50055bab766d9951b6c394759190d03311f3e9fcf194ca909e1 \
-    --hash=sha256:5d6850e6e36e332d5511a48a251790ddc545e16e8beaf046c03985c69ccb2676 \
-    --hash=sha256:6008adeca04a445ea6ef31b2cbaf1d01d02986047606f7da266629afee982630 \
-    --hash=sha256:64e723ca82a84053dd7bfcc986bdb34af8d9da83c521c19d6b472bc6880e191a \
-    --hash=sha256:6b00e21f86598b6330f0019b40fb397e705135040dbedc2ca9a93c7441178e74 \
-    --hash=sha256:6d224f0c4c9c98290a6990259073f496fcec1b5cc613eecbd22786d398ded3ad \
-    --hash=sha256:6dceb61d40cbfcf45f51e59933c784a50846dc03211054bd76b421a713dcdf19 \
-    --hash=sha256:7ac8f8eb153724f84885a1374999b7e45734bf93a87d8df1e7ce2146860edef6 \
-    --hash=sha256:85ccc5fa54c2ed64bd91ed3b4a627b9cce04646a659512a051fa82a92c04a448 \
-    --hash=sha256:869b5046d41abfea3e381dd143407b0d29b8282a904a19cb908fa24d090cc018 \
-    --hash=sha256:8bdb0285a0202888d19ec6b6d23d5990410decb932b709f2b0dfe216d031d218 \
-    --hash=sha256:8dfc5e195bbef80aabd81596ef52a1277ee7143fe419efc3c4d8ba2754671756 \
-    --hash=sha256:8e738a492b6221f8dcf281b67129510835461132b03024830ac0e554311a5c54 \
-    --hash=sha256:918440dea04521f499721c039863ef95433314b1db00ff826a02580c1f503e45 \
-    --hash=sha256:9641e21670c68c7e57d2053ddf6c443e4f0a6e18e547e86af3fad0795414a628 \
-    --hash=sha256:9d2f9d4cc2a53b38cabc2d6d80f7f9b7e3da26b2f53d48f05876fef7956b6968 \
-    --hash=sha256:a07f61fc452c43cd5328b392e52555f7d1952400a1ad09086c4a8addccbd138d \
-    --hash=sha256:a3277f5fa7483c927fe3a7b017b39351610265308f5267ac6d4c2b64cc1d8d25 \
-    --hash=sha256:a4a3907011d39dbc3e37bdc5df0a8c93853c369039b59efa33a7b6669de04c60 \
-    --hash=sha256:aeb2c2688ed93b027eb0d26aa188ada34acb22dceea256d76390eea135083950 \
-    --hash=sha256:b094116f0b6155e36a304ff912f89bbb5067157aff5f94060ff20bbabdc8da06 \
-    --hash=sha256:b8ffb498a83d7e0305968289441914154fb0ef5d8b3157df02a90c6695978295 \
-    --hash=sha256:b9bb62fac84d5f2ff523304e59e5c439955fb3b7f44e3d7b2085184db74d733b \
-    --hash=sha256:c61f66d93d712f6e03369b6a7769233bfda880b12f417eefdd4f16d1deb2fc4c \
-    --hash=sha256:ca6e61dc52f601d1d224526360cdeab0d0712ec104a2ce6cc5ccef6ed9a233bc \
-    --hash=sha256:ca7b26a5e456a843b9b6683eada193fc1f65c761b3a473941efe5a291f604c74 \
-    --hash=sha256:d12c923757de24e4e2110cf8832d83a886a4cf215c6e61ed506006872b43a6d1 \
-    --hash=sha256:d17bbc946f52ca67adf72a5ee783cd7cd3477f8f8796f59b4974a9b59cacc9ee \
-    --hash=sha256:dfd1e1b9f0898817babf840b77ce9fe655ecbe8b1b327983df485b30df8cc011 \
-    --hash=sha256:e0860a348bf7004c812c8368d1fc7f77fe8e4c095d661a579196a9533778e156 \
-    --hash=sha256:f2f5968608b1fe2a1d00d01ad1017ee27efd99b3437e08b83ded9b7af3f6f766 \
-    --hash=sha256:f3771b23bb3675a06f5d885c3630b1d01ea6cac9e84a01aaf5508706dba546c5 \
-    --hash=sha256:f68ef3660677e6624c8cace943e4765545f8191313a07288a53d3da188bd8581 \
-    --hash=sha256:f86f368e1c7ce897bf2457b9eb61169a44e2ef797099fb5728482b8d69f3f016 \
-    --hash=sha256:f90515974b39f4dea2f27c0959688621b46d96d5a626cf9c53dbc653a895c05c \
-    --hash=sha256:fe558371c1bdf3b8fa03e097c523fb9645b8730399c14fe7721ee9c9e2a545d3
-cryptography==42.0.1 \
-    --hash=sha256:0b7cacc142260ada944de070ce810c3e2a438963ee3deb45aa26fd2cee94c9a4 \
-    --hash=sha256:126e0ba3cc754b200a2fb88f67d66de0d9b9e94070c5bc548318c8dab6383cb6 \
-    --hash=sha256:160fa08dfa6dca9cb8ad9bd84e080c0db6414ba5ad9a7470bc60fb154f60111e \
-    --hash=sha256:16b9260d04a0bfc8952b00335ff54f471309d3eb9d7e8dbfe9b0bd9e26e67881 \
-    --hash=sha256:25ec6e9e81de5d39f111a4114193dbd39167cc4bbd31c30471cebedc2a92c323 \
-    --hash=sha256:265bdc693570b895eb641410b8fc9e8ddbce723a669236162b9d9cfb70bd8d77 \
-    --hash=sha256:2dff7a32880a51321f5de7869ac9dde6b1fca00fc1fef89d60e93f215468e824 \
-    --hash=sha256:2fe16624637d6e3e765530bc55caa786ff2cbca67371d306e5d0a72e7c3d0407 \
-    --hash=sha256:32ea63ceeae870f1a62e87f9727359174089f7b4b01e4999750827bf10e15d60 \
-    --hash=sha256:351db02c1938c8e6b1fee8a78d6b15c5ccceca7a36b5ce48390479143da3b411 \
-    --hash=sha256:430100abed6d3652208ae1dd410c8396213baee2e01a003a4449357db7dc9e14 \
-    --hash=sha256:4d84673c012aa698555d4710dcfe5f8a0ad76ea9dde8ef803128cc669640a2e0 \
-    --hash=sha256:50aecd93676bcca78379604ed664c45da82bc1241ffb6f97f6b7392ed5bc6f04 \
-    --hash=sha256:6ac8924085ed8287545cba89dc472fc224c10cc634cdf2c3e2866fe868108e77 \
-    --hash=sha256:6bfd823b336fdcd8e06285ae8883d3d2624d3bdef312a0e2ef905f332f8e9302 \
-    --hash=sha256:727387886c9c8de927c360a396c5edcb9340d9e960cda145fca75bdafdabd24c \
-    --hash=sha256:7911586fc69d06cd0ab3f874a169433db1bc2f0e40988661408ac06c4527a986 \
-    --hash=sha256:802d6f83233cf9696b59b09eb067e6b4d5ae40942feeb8e13b213c8fad47f1aa \
-    --hash=sha256:8d7efb6bf427d2add2f40b6e1e8e476c17508fa8907234775214b153e69c2e11 \
-    --hash=sha256:9544492e8024f29919eac2117edd8c950165e74eb551a22c53f6fdf6ba5f4cb8 \
-    --hash=sha256:95d900d19a370ae36087cc728e6e7be9c964ffd8cbcb517fd1efb9c9284a6abc \
-    --hash=sha256:9d61fcdf37647765086030d81872488e4cb3fafe1d2dda1d487875c3709c0a49 \
-    --hash=sha256:ab6b302d51fbb1dd339abc6f139a480de14d49d50f65fdc7dff782aa8631d035 \
-    --hash=sha256:b512f33c6ab195852595187af5440d01bb5f8dd57cb7a91e1e009a17f1b7ebca \
-    --hash=sha256:cb2861a9364fa27d24832c718150fdbf9ce6781d7dc246a516435f57cfa31fe7 \
-    --hash=sha256:d3594947d2507d4ef7a180a7f49a6db41f75fb874c2fd0e94f36b89bfd678bf2 \
-    --hash=sha256:d3902c779a92151f134f68e555dd0b17c658e13429f270d8a847399b99235a3f \
-    --hash=sha256:d50718dd574a49d3ef3f7ef7ece66ef281b527951eb2267ce570425459f6a404 \
-    --hash=sha256:e5edf189431b4d51f5c6fb4a95084a75cef6b4646c934eb6e32304fc720e1453 \
-    --hash=sha256:e6edc3a568667daf7d349d7e820783426ee4f1c0feab86c29bd1d6fe2755e009 \
-    --hash=sha256:ed1b2130f5456a09a134cc505a17fc2830a1a48ed53efd37dcc904a23d7b82fa \
-    --hash=sha256:fd33f53809bb363cf126bebe7a99d97735988d9b0131a2be59fbf83e1259a5b7
-cyclonedx-python-lib==6.4.0 \
-    --hash=sha256:1bcfea62211bc074b94dee05aa1fc2610e1bb6b8c507182073f4344e3e807b39 \
-    --hash=sha256:a877784f5f1066398336b61cdb7413311e93a6bc46a5065ba0d8e0dddbc54103
+cookiecutter==2.6.0 \
+    --hash=sha256:a54a8e37995e4ed963b3e82831072d1ad4b005af736bb17b99c2cbd9d41b6e2d \
+    --hash=sha256:db21f8169ea4f4fdc2408d48ca44859349de2647fbe494a9d6c3edfc0542c21c
+cookiecutter-python-vscode-github==0.6.0 \
+    --hash=sha256:8ca46b34b9bb0349f9cdd3857a9b3c140ae62304c163d90d2ef00ae8b78d215e \
+    --hash=sha256:9cd603585718cf82c95d76a52cc91627457204ad5089f12829ad29f2ba6c2521
+coverage==7.4.4 \
+    --hash=sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c \
+    --hash=sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63 \
+    --hash=sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7 \
+    --hash=sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f \
+    --hash=sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8 \
+    --hash=sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf \
+    --hash=sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0 \
+    --hash=sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384 \
+    --hash=sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76 \
+    --hash=sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7 \
+    --hash=sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d \
+    --hash=sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70 \
+    --hash=sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f \
+    --hash=sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818 \
+    --hash=sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b \
+    --hash=sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d \
+    --hash=sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec \
+    --hash=sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083 \
+    --hash=sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2 \
+    --hash=sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9 \
+    --hash=sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd \
+    --hash=sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade \
+    --hash=sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e \
+    --hash=sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a \
+    --hash=sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227 \
+    --hash=sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87 \
+    --hash=sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c \
+    --hash=sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e \
+    --hash=sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c \
+    --hash=sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e \
+    --hash=sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd \
+    --hash=sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec \
+    --hash=sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562 \
+    --hash=sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8 \
+    --hash=sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677 \
+    --hash=sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357 \
+    --hash=sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c \
+    --hash=sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd \
+    --hash=sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49 \
+    --hash=sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286 \
+    --hash=sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1 \
+    --hash=sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf \
+    --hash=sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51 \
+    --hash=sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409 \
+    --hash=sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384 \
+    --hash=sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e \
+    --hash=sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978 \
+    --hash=sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57 \
+    --hash=sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e \
+    --hash=sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2 \
+    --hash=sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48 \
+    --hash=sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4
+cryptography==42.0.5 \
+    --hash=sha256:0270572b8bd2c833c3981724b8ee9747b3ec96f699a9665470018594301439ee \
+    --hash=sha256:111a0d8553afcf8eb02a4fea6ca4f59d48ddb34497aa8706a6cf536f1a5ec576 \
+    --hash=sha256:16a48c23a62a2f4a285699dba2e4ff2d1cff3115b9df052cdd976a18856d8e3d \
+    --hash=sha256:1b95b98b0d2af784078fa69f637135e3c317091b615cd0905f8b8a087e86fa30 \
+    --hash=sha256:1f71c10d1e88467126f0efd484bd44bca5e14c664ec2ede64c32f20875c0d413 \
+    --hash=sha256:2424ff4c4ac7f6b8177b53c17ed5d8fa74ae5955656867f5a8affaca36a27abb \
+    --hash=sha256:2bce03af1ce5a5567ab89bd90d11e7bbdff56b8af3acbbec1faded8f44cb06da \
+    --hash=sha256:329906dcc7b20ff3cad13c069a78124ed8247adcac44b10bea1130e36caae0b4 \
+    --hash=sha256:37dd623507659e08be98eec89323469e8c7b4c1407c85112634ae3dbdb926fdd \
+    --hash=sha256:3eaafe47ec0d0ffcc9349e1708be2aaea4c6dd4978d76bf6eb0cb2c13636c6fc \
+    --hash=sha256:5e6275c09d2badf57aea3afa80d975444f4be8d3bc58f7f80d2a484c6f9485c8 \
+    --hash=sha256:6fe07eec95dfd477eb9530aef5bead34fec819b3aaf6c5bd6d20565da607bfe1 \
+    --hash=sha256:7367d7b2eca6513681127ebad53b2582911d1736dc2ffc19f2c3ae49997496bc \
+    --hash=sha256:7cde5f38e614f55e28d831754e8a3bacf9ace5d1566235e39d91b35502d6936e \
+    --hash=sha256:9481ffe3cf013b71b2428b905c4f7a9a4f76ec03065b05ff499bb5682a8d9ad8 \
+    --hash=sha256:98d8dc6d012b82287f2c3d26ce1d2dd130ec200c8679b6213b3c73c08b2b7940 \
+    --hash=sha256:a011a644f6d7d03736214d38832e030d8268bcff4a41f728e6030325fea3e400 \
+    --hash=sha256:a2913c5375154b6ef2e91c10b5720ea6e21007412f6437504ffea2109b5a33d7 \
+    --hash=sha256:a30596bae9403a342c978fb47d9b0ee277699fa53bbafad14706af51fe543d16 \
+    --hash=sha256:b03c2ae5d2f0fc05f9a2c0c997e1bc18c8229f392234e8a0194f202169ccd278 \
+    --hash=sha256:b6cd2203306b63e41acdf39aa93b86fb566049aeb6dc489b70e34bcd07adca74 \
+    --hash=sha256:b7ffe927ee6531c78f81aa17e684e2ff617daeba7f189f911065b2ea2d526dec \
+    --hash=sha256:b8cac287fafc4ad485b8a9b67d0ee80c66bf3574f655d3b97ef2e1082360faf1 \
+    --hash=sha256:ba334e6e4b1d92442b75ddacc615c5476d4ad55cc29b15d590cc6b86efa487e2 \
+    --hash=sha256:ba3e4a42397c25b7ff88cdec6e2a16c2be18720f317506ee25210f6d31925f9c \
+    --hash=sha256:c41fb5e6a5fe9ebcd58ca3abfeb51dffb5d83d6775405305bfa8715b76521922 \
+    --hash=sha256:cd2030f6650c089aeb304cf093f3244d34745ce0cfcc39f20c6fbfe030102e2a \
+    --hash=sha256:cd65d75953847815962c84a4654a84850b2bb4aed3f26fadcc1c13892e1e29f6 \
+    --hash=sha256:e4985a790f921508f36f81831817cbc03b102d643b5fcb81cd33df3fa291a1a1 \
+    --hash=sha256:e807b3188f9eb0eaa7bbb579b462c5ace579f1cedb28107ce8b48a9f7ad3679e \
+    --hash=sha256:f12764b8fffc7a123f641d7d049d382b73f96a34117e0b637b80643169cec8ac \
+    --hash=sha256:f8837fe1d6ac4a8052a9a8ddab256bc006242696f03368a4009be7ee3075cdb7
+cyclonedx-python-lib==6.4.4 \
+    --hash=sha256:1b6f9109b6b9e91636dff822c2de90a05c0c8af120317713c1b879dbfdebdff8 \
+    --hash=sha256:c366619cc4effd528675f1f7a7a00be30b6695ff03f49c64880ad15acbebc341
 defusedxml==0.7.1 \
     --hash=sha256:1bb3032db185915b62d7c6209c5a8792be6a32ab2fedacc84e01b52c51aa3e69 \
     --hash=sha256:a352e7e428770286cc899e2542b6cdaedb2b4953ff269a210103ec58f6198a61
 dill==0.3.8 \
     --hash=sha256:3ebe3c479ad625c4553aca177444d89b486b1d84982eeacded644afc0cf797ca \
     --hash=sha256:c36ca9ffb54365bdd2f8eb3eff7d2a21237f8452b57ace88b1ac615b7e815bd7
 distlib==0.3.8 \
     --hash=sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784 \
     --hash=sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64
 docformatter==1.7.5 \
     --hash=sha256:a24f5545ed1f30af00d106f5d85dc2fce4959295687c24c8f39f5263afaf9186 \
     --hash=sha256:ffed3da0daffa2e77f80ccba4f0e50bfa2755e1c10e130102571c890a61b246e
-docutils==0.20.1 \
-    --hash=sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6 \
-    --hash=sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b
-filelock==3.13.1 \
-    --hash=sha256:521f5f56c50f8426f5e03ad3b281b490a87ef15bc6c526f168290f0c7148d44e \
-    --hash=sha256:57dbda9b35157b05fb3e58ee91448612eb674172fab98ee235ccb0b5bee19a1c
+docutils==0.21.1 \
+    --hash=sha256:14c8d34a55b46c88f9f714adb29cefbdd69fb82f3fef825e59c5faab935390d8 \
+    --hash=sha256:65249d8a5345bc95e0f40f280ba63c98eb24de35c6c8f5b662e3e8948adea83f
+filelock==3.13.4 \
+    --hash=sha256:404e5e9253aa60ad457cae1be07c0f0ca90a63931200a47d9b6a6af84fd7b45f \
+    --hash=sha256:d13f466618bfde72bd2c18255e269f72542c6e70e7bac83a0232d6b1cc5c8cf4
 flake8==7.0.0 \
     --hash=sha256:33f96621059e65eec474169085dc92bf26e7b2d47366b70be2f67ab80dc25132 \
     --hash=sha256:a6dfbb75e03252917f2473ea9653f7cd799c3064e54d4c8140044c5c065f53c3
 flake8-bandit==4.1.1 \
     --hash=sha256:068e09287189cbfd7f986e92605adea2067630b75380c6b5733dab7d87f9a84e \
     --hash=sha256:4c8a53eb48f23d4ef1e59293657181a3c989d0077c9952717e98a0eace43e06d
 html5lib==1.1 \
     --hash=sha256:0d78f8fde1c230e99fe37986a60526d7049ed4bf8a9fadbad5f00e22e58e041d \
     --hash=sha256:b2e5b40261e20f354d198eae92afc10d750afb487ed5e50f9c4eaf07c184146f
-identify==2.5.33 \
-    --hash=sha256:161558f9fe4559e1557e1bff323e8631f6a0e4837f7497767c1782832f16b62d \
-    --hash=sha256:d40ce5fcd762817627670da8a7d8d8e65f24342d14539c59488dc603bf662e34
-idna==3.6 \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
-importlib-metadata==7.0.1 \
-    --hash=sha256:4805911c3a4ec7c3966410053e9ec6a1fecd629117df5adee56dfc9432a1081e \
-    --hash=sha256:f238736bb06590ae52ac1fab06a3a9ef1d8dce2b7a35b5ab329371d6c8f5d2cc
+identify==2.5.35 \
+    --hash=sha256:10a7ca245cfcd756a554a7288159f72ff105ad233c7c4b9c6f0f4d108f5f6791 \
+    --hash=sha256:c4de0081837b211594f8e877a6b4fad7ca32bbfc1a9307fdd61c28bfe923f13e
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
+importlib-metadata==7.1.0 \
+    --hash=sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570 \
+    --hash=sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
 isort==5.13.2 \
     --hash=sha256:48fdfcb9face5d58a4f6dde2e72a1fb8dcaf8ab26f95ab49fab84c2ddefb0109 \
     --hash=sha256:8ca5e72a8d85860d5a3fa69b8745237f2939afe12dbf656afbcb47fe72d947a6
-jaraco-classes==3.3.0 \
-    --hash=sha256:10afa92b6743f25c0cf5f37c6bb6e18e2c5bb84a16527ccfc0040ea377e7aaeb \
-    --hash=sha256:c063dd08e89217cee02c8d5e5ec560f2c8ce6cdc2fcdc2e68f7b2e5547ed3621
+jaraco-classes==3.4.0 \
+    --hash=sha256:47a024b51d0239c0dd8c8540c6c7f484be3b8fcf0b2d85c13825780d3b3f3acd \
+    --hash=sha256:f662826b6bed8cace05e7ff873ce0f9283b5c924470fe664fff1c2f00f581790
+jaraco-context==5.3.0 \
+    --hash=sha256:3e16388f7da43d384a1a7cd3452e72e14732ac9fe459678773a3608a812bf266 \
+    --hash=sha256:c2f67165ce1f9be20f32f650f25d8edfc1646a8aeee48ae06fb35f90763576d2
+jaraco-functools==4.0.0 \
+    --hash=sha256:c279cb24c93d694ef7270f970d499cab4d3813f4e08273f95398651a634f0925 \
+    --hash=sha256:daf276ddf234bea897ef14f43c4e1bf9eefeac7b7a82a4dd69228ac20acff68d
 jeepney==0.8.0 \
     --hash=sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806 \
     --hash=sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755
 jinja2==3.1.3 \
     --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
     --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
-keyring==24.3.0 \
-    --hash=sha256:4446d35d636e6a10b8bce7caa66913dd9eca5fd222ca03a3d42c38608ac30836 \
-    --hash=sha256:e730ecffd309658a08ee82535a3b5ec4b4c8669a9be11efb66249d8e0aeb9a25
-license-expression==30.2.0 \
-    --hash=sha256:1a7dc2bb2d09cdc983d072e4f9adc787e107e09def84cbb3919baaaf4f8e6fa1 \
-    --hash=sha256:599928edd995c43fc335e0af342076144dc71cb858afa1ed9c1c30c4e81794f5
+keyring==25.1.0 \
+    --hash=sha256:26fc12e6a329d61d24aa47b22a7c5c3f35753df7d8f2860973cf94f4e1fb3427 \
+    --hash=sha256:7230ea690525133f6ad536a9b5def74a4bd52642abe594761028fc044d7c7893
+license-expression==30.3.0 \
+    --hash=sha256:1295406f736b4f395ff069aec1cebfad53c0fcb3cf57df0f5ec58fc7b905aea5 \
+    --hash=sha256:ae0ba9a829d6909c785dc2f0131f13d10d68318e4a5f28af5ef152d6b52f9b41
 markdown-it-py==3.0.0 \
     --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
     --hash=sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb
-markupsafe==2.1.4 \
-    --hash=sha256:0042d6a9880b38e1dd9ff83146cc3c9c18a059b9360ceae207805567aacccc69 \
-    --hash=sha256:0c26f67b3fe27302d3a412b85ef696792c4a2386293c53ba683a89562f9399b0 \
-    --hash=sha256:0fbad3d346df8f9d72622ac71b69565e621ada2ce6572f37c2eae8dacd60385d \
-    --hash=sha256:15866d7f2dc60cfdde12ebb4e75e41be862348b4728300c36cdf405e258415ec \
-    --hash=sha256:1c98c33ffe20e9a489145d97070a435ea0679fddaabcafe19982fe9c971987d5 \
-    --hash=sha256:21e7af8091007bf4bebf4521184f4880a6acab8df0df52ef9e513d8e5db23411 \
-    --hash=sha256:23984d1bdae01bee794267424af55eef4dfc038dc5d1272860669b2aa025c9e3 \
-    --hash=sha256:31f57d64c336b8ccb1966d156932f3daa4fee74176b0fdc48ef580be774aae74 \
-    --hash=sha256:3583a3a3ab7958e354dc1d25be74aee6228938312ee875a22330c4dc2e41beb0 \
-    --hash=sha256:36d7626a8cca4d34216875aee5a1d3d654bb3dac201c1c003d182283e3205949 \
-    --hash=sha256:396549cea79e8ca4ba65525470d534e8a41070e6b3500ce2414921099cb73e8d \
-    --hash=sha256:3a66c36a3864df95e4f62f9167c734b3b1192cb0851b43d7cc08040c074c6279 \
-    --hash=sha256:3aae9af4cac263007fd6309c64c6ab4506dd2b79382d9d19a1994f9240b8db4f \
-    --hash=sha256:3ab3a886a237f6e9c9f4f7d272067e712cdb4efa774bef494dccad08f39d8ae6 \
-    --hash=sha256:47bb5f0142b8b64ed1399b6b60f700a580335c8e1c57f2f15587bd072012decc \
-    --hash=sha256:49a3b78a5af63ec10d8604180380c13dcd870aba7928c1fe04e881d5c792dc4e \
-    --hash=sha256:4df98d4a9cd6a88d6a585852f56f2155c9cdb6aec78361a19f938810aa020954 \
-    --hash=sha256:5045e892cfdaecc5b4c01822f353cf2c8feb88a6ec1c0adef2a2e705eef0f656 \
-    --hash=sha256:5244324676254697fe5c181fc762284e2c5fceeb1c4e3e7f6aca2b6f107e60dc \
-    --hash=sha256:54635102ba3cf5da26eb6f96c4b8c53af8a9c0d97b64bdcb592596a6255d8518 \
-    --hash=sha256:54a7e1380dfece8847c71bf7e33da5d084e9b889c75eca19100ef98027bd9f56 \
-    --hash=sha256:55d03fea4c4e9fd0ad75dc2e7e2b6757b80c152c032ea1d1de487461d8140efc \
-    --hash=sha256:698e84142f3f884114ea8cf83e7a67ca8f4ace8454e78fe960646c6c91c63bfa \
-    --hash=sha256:6aa5e2e7fc9bc042ae82d8b79d795b9a62bd8f15ba1e7594e3db243f158b5565 \
-    --hash=sha256:7653fa39578957bc42e5ebc15cf4361d9e0ee4b702d7d5ec96cdac860953c5b4 \
-    --hash=sha256:765f036a3d00395a326df2835d8f86b637dbaf9832f90f5d196c3b8a7a5080cb \
-    --hash=sha256:78bc995e004681246e85e28e068111a4c3f35f34e6c62da1471e844ee1446250 \
-    --hash=sha256:7a07f40ef8f0fbc5ef1000d0c78771f4d5ca03b4953fc162749772916b298fc4 \
-    --hash=sha256:8b570a1537367b52396e53325769608f2a687ec9a4363647af1cded8928af959 \
-    --hash=sha256:987d13fe1d23e12a66ca2073b8d2e2a75cec2ecb8eab43ff5624ba0ad42764bc \
-    --hash=sha256:9896fca4a8eb246defc8b2a7ac77ef7553b638e04fbf170bff78a40fa8a91474 \
-    --hash=sha256:9e9e3c4020aa2dc62d5dd6743a69e399ce3de58320522948af6140ac959ab863 \
-    --hash=sha256:a0b838c37ba596fcbfca71651a104a611543077156cb0a26fe0c475e1f152ee8 \
-    --hash=sha256:a4d176cfdfde84f732c4a53109b293d05883e952bbba68b857ae446fa3119b4f \
-    --hash=sha256:a76055d5cb1c23485d7ddae533229039b850db711c554a12ea64a0fd8a0129e2 \
-    --hash=sha256:a76cd37d229fc385738bd1ce4cba2a121cf26b53864c1772694ad0ad348e509e \
-    --hash=sha256:a7cc49ef48a3c7a0005a949f3c04f8baa5409d3f663a1b36f0eba9bfe2a0396e \
-    --hash=sha256:abf5ebbec056817057bfafc0445916bb688a255a5146f900445d081db08cbabb \
-    --hash=sha256:b0fe73bac2fed83839dbdbe6da84ae2a31c11cfc1c777a40dbd8ac8a6ed1560f \
-    --hash=sha256:b6f14a9cd50c3cb100eb94b3273131c80d102e19bb20253ac7bd7336118a673a \
-    --hash=sha256:b83041cda633871572f0d3c41dddd5582ad7d22f65a72eacd8d3d6d00291df26 \
-    --hash=sha256:b835aba863195269ea358cecc21b400276747cc977492319fd7682b8cd2c253d \
-    --hash=sha256:bf1196dcc239e608605b716e7b166eb5faf4bc192f8a44b81e85251e62584bd2 \
-    --hash=sha256:c669391319973e49a7c6230c218a1e3044710bc1ce4c8e6eb71f7e6d43a2c131 \
-    --hash=sha256:c7556bafeaa0a50e2fe7dc86e0382dea349ebcad8f010d5a7dc6ba568eaaa789 \
-    --hash=sha256:c8f253a84dbd2c63c19590fa86a032ef3d8cc18923b8049d91bcdeeb2581fbf6 \
-    --hash=sha256:d18b66fe626ac412d96c2ab536306c736c66cf2a31c243a45025156cc190dc8a \
-    --hash=sha256:d5291d98cd3ad9a562883468c690a2a238c4a6388ab3bd155b0c75dd55ece858 \
-    --hash=sha256:d5c31fe855c77cad679b302aabc42d724ed87c043b1432d457f4976add1c2c3e \
-    --hash=sha256:d6e427c7378c7f1b2bef6a344c925b8b63623d3321c09a237b7cc0e77dd98ceb \
-    --hash=sha256:dac1ebf6983148b45b5fa48593950f90ed6d1d26300604f321c74a9ca1609f8e \
-    --hash=sha256:de8153a7aae3835484ac168a9a9bdaa0c5eee4e0bc595503c95d53b942879c84 \
-    --hash=sha256:e1a0d1924a5013d4f294087e00024ad25668234569289650929ab871231668e7 \
-    --hash=sha256:e7902211afd0af05fbadcc9a312e4cf10f27b779cf1323e78d52377ae4b72bea \
-    --hash=sha256:e888ff76ceb39601c59e219f281466c6d7e66bd375b4ec1ce83bcdc68306796b \
-    --hash=sha256:f06e5a9e99b7df44640767842f414ed5d7bedaaa78cd817ce04bbd6fd86e2dd6 \
-    --hash=sha256:f6be2d708a9d0e9b0054856f07ac7070fbe1754be40ca8525d5adccdbda8f475 \
-    --hash=sha256:f9917691f410a2e0897d1ef99619fd3f7dd503647c8ff2475bf90c3cf222ad74 \
-    --hash=sha256:fc1a75aa8f11b87910ffd98de62b29d6520b6d6e8a3de69a70ca34dea85d2a8a \
-    --hash=sha256:fe8512ed897d5daf089e5bd010c3dc03bb1bdae00b35588c49b98268d4a01e00
+markupsafe==2.1.5 \
+    --hash=sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf \
+    --hash=sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff \
+    --hash=sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f \
+    --hash=sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3 \
+    --hash=sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532 \
+    --hash=sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f \
+    --hash=sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617 \
+    --hash=sha256:2d2d793e36e230fd32babe143b04cec8a8b3eb8a3122d2aceb4a371e6b09b8df \
+    --hash=sha256:30b600cf0a7ac9234b2638fbc0fb6158ba5bdcdf46aeb631ead21248b9affbc4 \
+    --hash=sha256:397081c1a0bfb5124355710fe79478cdbeb39626492b15d399526ae53422b906 \
+    --hash=sha256:3a57fdd7ce31c7ff06cdfbf31dafa96cc533c21e443d57f5b1ecc6cdc668ec7f \
+    --hash=sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4 \
+    --hash=sha256:3e53af139f8579a6d5f7b76549125f0d94d7e630761a2111bc431fd820e163b8 \
+    --hash=sha256:4096e9de5c6fdf43fb4f04c26fb114f61ef0bf2e5604b6ee3019d51b69e8c371 \
+    --hash=sha256:4275d846e41ecefa46e2015117a9f491e57a71ddd59bbead77e904dc02b1bed2 \
+    --hash=sha256:4c31f53cdae6ecfa91a77820e8b151dba54ab528ba65dfd235c80b086d68a465 \
+    --hash=sha256:4f11aa001c540f62c6166c7726f71f7573b52c68c31f014c25cc7901deea0b52 \
+    --hash=sha256:5049256f536511ee3f7e1b3f87d1d1209d327e818e6ae1365e8653d7e3abb6a6 \
+    --hash=sha256:58c98fee265677f63a4385256a6d7683ab1832f3ddd1e66fe948d5880c21a169 \
+    --hash=sha256:598e3276b64aff0e7b3451b72e94fa3c238d452e7ddcd893c3ab324717456bad \
+    --hash=sha256:5b7b716f97b52c5a14bffdf688f971b2d5ef4029127f1ad7a513973cfd818df2 \
+    --hash=sha256:5dedb4db619ba5a2787a94d877bc8ffc0566f92a01c0ef214865e54ecc9ee5e0 \
+    --hash=sha256:619bc166c4f2de5caa5a633b8b7326fbe98e0ccbfacabd87268a2b15ff73a029 \
+    --hash=sha256:629ddd2ca402ae6dbedfceeba9c46d5f7b2a61d9749597d4307f943ef198fc1f \
+    --hash=sha256:656f7526c69fac7f600bd1f400991cc282b417d17539a1b228617081106feb4a \
+    --hash=sha256:6ec585f69cec0aa07d945b20805be741395e28ac1627333b1c5b0105962ffced \
+    --hash=sha256:72b6be590cc35924b02c78ef34b467da4ba07e4e0f0454a2c5907f473fc50ce5 \
+    --hash=sha256:7502934a33b54030eaf1194c21c692a534196063db72176b0c4028e140f8f32c \
+    --hash=sha256:7a68b554d356a91cce1236aa7682dc01df0edba8d043fd1ce607c49dd3c1edcf \
+    --hash=sha256:7b2e5a267c855eea6b4283940daa6e88a285f5f2a67f2220203786dfa59b37e9 \
+    --hash=sha256:823b65d8706e32ad2df51ed89496147a42a2a6e01c13cfb6ffb8b1e92bc910bb \
+    --hash=sha256:8590b4ae07a35970728874632fed7bd57b26b0102df2d2b233b6d9d82f6c62ad \
+    --hash=sha256:8dd717634f5a044f860435c1d8c16a270ddf0ef8588d4887037c5028b859b0c3 \
+    --hash=sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1 \
+    --hash=sha256:97cafb1f3cbcd3fd2b6fbfb99ae11cdb14deea0736fc2b0952ee177f2b813a46 \
+    --hash=sha256:a17a92de5231666cfbe003f0e4b9b3a7ae3afb1ec2845aadc2bacc93ff85febc \
+    --hash=sha256:a549b9c31bec33820e885335b451286e2969a2d9e24879f83fe904a5ce59d70a \
+    --hash=sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee \
+    --hash=sha256:ae2ad8ae6ebee9d2d94b17fb62763125f3f374c25618198f40cbb8b525411900 \
+    --hash=sha256:b91c037585eba9095565a3556f611e3cbfaa42ca1e865f7b8015fe5c7336d5a5 \
+    --hash=sha256:bc1667f8b83f48511b94671e0e441401371dfd0f0a795c7daa4a3cd1dde55bea \
+    --hash=sha256:bec0a414d016ac1a18862a519e54b2fd0fc8bbfd6890376898a6c0891dd82e9f \
+    --hash=sha256:bf50cd79a75d181c9181df03572cdce0fbb75cc353bc350712073108cba98de5 \
+    --hash=sha256:bff1b4290a66b490a2f4719358c0cdcd9bafb6b8f061e45c7a2460866bf50c2e \
+    --hash=sha256:c061bb86a71b42465156a3ee7bd58c8c2ceacdbeb95d05a99893e08b8467359a \
+    --hash=sha256:c8b29db45f8fe46ad280a7294f5c3ec36dbac9491f2d1c17345be8e69cc5928f \
+    --hash=sha256:ce409136744f6521e39fd8e2a24c53fa18ad67aa5bc7c2cf83645cce5b5c4e50 \
+    --hash=sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a \
+    --hash=sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b \
+    --hash=sha256:d9fad5155d72433c921b782e58892377c44bd6252b5af2f67f16b194987338a4 \
+    --hash=sha256:daa4ee5a243f0f20d528d939d06670a298dd39b1ad5f8a72a4275124a7819eff \
+    --hash=sha256:db0b55e0f3cc0be60c1f19efdde9a637c32740486004f20d1cff53c3c0ece4d2 \
+    --hash=sha256:e61659ba32cf2cf1481e575d0462554625196a1f2fc06a1c777d3f48e8865d46 \
+    --hash=sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b \
+    --hash=sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf \
+    --hash=sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5 \
+    --hash=sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5 \
+    --hash=sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab \
+    --hash=sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd \
+    --hash=sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68
 mccabe==0.7.0 \
     --hash=sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325 \
     --hash=sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e
 mdurl==0.1.2 \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
 more-itertools==10.2.0 \
     --hash=sha256:686b06abe565edfab151cb8fd385a05651e1fdf8f0a14191e4439283421f8684 \
     --hash=sha256:8fccb480c43d3e99a00087634c06dd02b0d50fbf088b380de5a41a015ec239e1
-msgpack==1.0.7 \
-    --hash=sha256:04ad6069c86e531682f9e1e71b71c1c3937d6014a7c3e9edd2aa81ad58842862 \
-    --hash=sha256:0bfdd914e55e0d2c9e1526de210f6fe8ffe9705f2b1dfcc4aecc92a4cb4b533d \
-    --hash=sha256:1dc93e8e4653bdb5910aed79f11e165c85732067614f180f70534f056da97db3 \
-    --hash=sha256:1e2d69948e4132813b8d1131f29f9101bc2c915f26089a6d632001a5c1349672 \
-    --hash=sha256:235a31ec7db685f5c82233bddf9858748b89b8119bf4538d514536c485c15fe0 \
-    --hash=sha256:27dcd6f46a21c18fa5e5deed92a43d4554e3df8d8ca5a47bf0615d6a5f39dbc9 \
-    --hash=sha256:28efb066cde83c479dfe5a48141a53bc7e5f13f785b92ddde336c716663039ee \
-    --hash=sha256:3476fae43db72bd11f29a5147ae2f3cb22e2f1a91d575ef130d2bf49afd21c46 \
-    --hash=sha256:36e17c4592231a7dbd2ed09027823ab295d2791b3b1efb2aee874b10548b7524 \
-    --hash=sha256:384d779f0d6f1b110eae74cb0659d9aa6ff35aaf547b3955abf2ab4c901c4819 \
-    --hash=sha256:38949d30b11ae5f95c3c91917ee7a6b239f5ec276f271f28638dec9156f82cfc \
-    --hash=sha256:3967e4ad1aa9da62fd53e346ed17d7b2e922cba5ab93bdd46febcac39be636fc \
-    --hash=sha256:3e7bf4442b310ff154b7bb9d81eb2c016b7d597e364f97d72b1acc3817a0fdc1 \
-    --hash=sha256:3f0c8c6dfa6605ab8ff0611995ee30d4f9fcff89966cf562733b4008a3d60d82 \
-    --hash=sha256:484ae3240666ad34cfa31eea7b8c6cd2f1fdaae21d73ce2974211df099a95d81 \
-    --hash=sha256:4a7b4f35de6a304b5533c238bee86b670b75b03d31b7797929caa7a624b5dda6 \
-    --hash=sha256:4cb14ce54d9b857be9591ac364cb08dc2d6a5c4318c1182cb1d02274029d590d \
-    --hash=sha256:4e71bc4416de195d6e9b4ee93ad3f2f6b2ce11d042b4d7a7ee00bbe0358bd0c2 \
-    --hash=sha256:52700dc63a4676669b341ba33520f4d6e43d3ca58d422e22ba66d1736b0a6e4c \
-    --hash=sha256:572efc93db7a4d27e404501975ca6d2d9775705c2d922390d878fcf768d92c87 \
-    --hash=sha256:576eb384292b139821c41995523654ad82d1916da6a60cff129c715a6223ea84 \
-    --hash=sha256:5b0bf0effb196ed76b7ad883848143427a73c355ae8e569fa538365064188b8e \
-    --hash=sha256:5b6ccc0c85916998d788b295765ea0e9cb9aac7e4a8ed71d12e7d8ac31c23c95 \
-    --hash=sha256:5ed82f5a7af3697b1c4786053736f24a0efd0a1b8a130d4c7bfee4b9ded0f08f \
-    --hash=sha256:6d4c80667de2e36970ebf74f42d1088cc9ee7ef5f4e8c35eee1b40eafd33ca5b \
-    --hash=sha256:730076207cb816138cf1af7f7237b208340a2c5e749707457d70705715c93b93 \
-    --hash=sha256:7687e22a31e976a0e7fc99c2f4d11ca45eff652a81eb8c8085e9609298916dcf \
-    --hash=sha256:822ea70dc4018c7e6223f13affd1c5c30c0f5c12ac1f96cd8e9949acddb48a61 \
-    --hash=sha256:84b0daf226913133f899ea9b30618722d45feffa67e4fe867b0b5ae83a34060c \
-    --hash=sha256:85765fdf4b27eb5086f05ac0491090fc76f4f2b28e09d9350c31aac25a5aaff8 \
-    --hash=sha256:8dd178c4c80706546702c59529ffc005681bd6dc2ea234c450661b205445a34d \
-    --hash=sha256:8f5b234f567cf76ee489502ceb7165c2a5cecec081db2b37e35332b537f8157c \
-    --hash=sha256:98bbd754a422a0b123c66a4c341de0474cad4a5c10c164ceed6ea090f3563db4 \
-    --hash=sha256:993584fc821c58d5993521bfdcd31a4adf025c7d745bbd4d12ccfecf695af5ba \
-    --hash=sha256:a40821a89dc373d6427e2b44b572efc36a2778d3f543299e2f24eb1a5de65415 \
-    --hash=sha256:b291f0ee7961a597cbbcc77709374087fa2a9afe7bdb6a40dbbd9b127e79afee \
-    --hash=sha256:b573a43ef7c368ba4ea06050a957c2a7550f729c31f11dd616d2ac4aba99888d \
-    --hash=sha256:b610ff0f24e9f11c9ae653c67ff8cc03c075131401b3e5ef4b82570d1728f8a9 \
-    --hash=sha256:bdf38ba2d393c7911ae989c3bbba510ebbcdf4ecbdbfec36272abe350c454075 \
-    --hash=sha256:bfef2bb6ef068827bbd021017a107194956918ab43ce4d6dc945ffa13efbc25f \
-    --hash=sha256:cab3db8bab4b7e635c1c97270d7a4b2a90c070b33cbc00c99ef3f9be03d3e1f7 \
-    --hash=sha256:cb70766519500281815dfd7a87d3a178acf7ce95390544b8c90587d76b227681 \
-    --hash=sha256:cca1b62fe70d761a282496b96a5e51c44c213e410a964bdffe0928e611368329 \
-    --hash=sha256:ccf9a39706b604d884d2cb1e27fe973bc55f2890c52f38df742bc1d79ab9f5e1 \
-    --hash=sha256:dc43f1ec66eb8440567186ae2f8c447d91e0372d793dfe8c222aec857b81a8cf \
-    --hash=sha256:dd632777ff3beaaf629f1ab4396caf7ba0bdd075d948a69460d13d44357aca4c \
-    --hash=sha256:e45ae4927759289c30ccba8d9fdce62bb414977ba158286b5ddaf8df2cddb5c5 \
-    --hash=sha256:e50ebce52f41370707f1e21a59514e3375e3edd6e1832f5e5235237db933c98b \
-    --hash=sha256:ebbbba226f0a108a7366bf4b59bf0f30a12fd5e75100c630267d94d7f0ad20e5 \
-    --hash=sha256:ec79ff6159dffcc30853b2ad612ed572af86c92b5168aa3fc01a67b0fa40665e \
-    --hash=sha256:f0936e08e0003f66bfd97e74ee530427707297b0d0361247e9b4f59ab78ddc8b \
-    --hash=sha256:f26a07a6e877c76a88e3cecac8531908d980d3d5067ff69213653649ec0f60ad \
-    --hash=sha256:f64e376cd20d3f030190e8c32e1c64582eba56ac6dc7d5b0b49a9d44021b52fd \
-    --hash=sha256:f6ffbc252eb0d229aeb2f9ad051200668fc3a9aaa8994e49f0cb2ffe2b7867e7 \
-    --hash=sha256:f9a7c509542db4eceed3dcf21ee5267ab565a83555c9b88a8109dcecc4709002 \
-    --hash=sha256:ff1d0899f104f3921d94579a5638847f783c9b04f2d5f229392ca77fba5b82fc
-mypy==1.8.0 \
-    --hash=sha256:028cf9f2cae89e202d7b6593cd98db6759379f17a319b5faf4f9978d7084cdc6 \
-    --hash=sha256:2afecd6354bbfb6e0160f4e4ad9ba6e4e003b767dd80d85516e71f2e955ab50d \
-    --hash=sha256:2b5b6c721bd4aabaadead3a5e6fa85c11c6c795e0c81a7215776ef8afc66de02 \
-    --hash=sha256:42419861b43e6962a649068a61f4a4839205a3ef525b858377a960b9e2de6e0d \
-    --hash=sha256:42c6680d256ab35637ef88891c6bd02514ccb7e1122133ac96055ff458f93fc3 \
-    --hash=sha256:485a8942f671120f76afffff70f259e1cd0f0cfe08f81c05d8816d958d4577d3 \
-    --hash=sha256:4c886c6cce2d070bd7df4ec4a05a13ee20c0aa60cb587e8d1265b6c03cf91da3 \
-    --hash=sha256:4e6d97288757e1ddba10dd9549ac27982e3e74a49d8d0179fc14d4365c7add66 \
-    --hash=sha256:4ef4be7baf08a203170f29e89d79064463b7fc7a0908b9d0d5114e8009c3a259 \
-    --hash=sha256:51720c776d148bad2372ca21ca29256ed483aa9a4cdefefcef49006dff2a6835 \
-    --hash=sha256:52825b01f5c4c1c4eb0db253ec09c7aa17e1a7304d247c48b6f3599ef40db8bd \
-    --hash=sha256:538fd81bb5e430cc1381a443971c0475582ff9f434c16cd46d2c66763ce85d9d \
-    --hash=sha256:5c1538c38584029352878a0466f03a8ee7547d7bd9f641f57a0f3017a7c905b8 \
-    --hash=sha256:6ff8b244d7085a0b425b56d327b480c3b29cafbd2eff27316a004f9a7391ae07 \
-    --hash=sha256:7178def594014aa6c35a8ff411cf37d682f428b3b5617ca79029d8ae72f5402b \
-    --hash=sha256:720a5ca70e136b675af3af63db533c1c8c9181314d207568bbe79051f122669e \
-    --hash=sha256:7f1478736fcebb90f97e40aff11a5f253af890c845ee0c850fe80aa060a267c6 \
-    --hash=sha256:855fe27b80375e5c5878492f0729540db47b186509c98dae341254c8f45f42ae \
-    --hash=sha256:8963b83d53ee733a6e4196954502b33567ad07dfd74851f32be18eb932fb1cb9 \
-    --hash=sha256:9261ed810972061388918c83c3f5cd46079d875026ba97380f3e3978a72f503d \
-    --hash=sha256:99b00bc72855812a60d253420d8a2eae839b0afa4938f09f4d2aa9bb4654263a \
-    --hash=sha256:ab3c84fa13c04aeeeabb2a7f67a25ef5d77ac9d6486ff33ded762ef353aa5592 \
-    --hash=sha256:afe3fe972c645b4632c563d3f3eff1cdca2fa058f730df2b93a35e3b0c538218 \
-    --hash=sha256:d19c413b3c07cbecf1f991e2221746b0d2a9410b59cb3f4fb9557f0365a1a817 \
-    --hash=sha256:df9824ac11deaf007443e7ed2a4a26bebff98d2bc43c6da21b2b64185da011c4 \
-    --hash=sha256:e46f44b54ebddbeedbd3d5b289a893219065ef805d95094d16a0af6630f5d410 \
-    --hash=sha256:f5ac9a4eeb1ec0f1ccdc6f326bcdb464de5f80eb07fb38b5ddd7b0de6bc61e55
+msgpack==1.0.8 \
+    --hash=sha256:00e073efcba9ea99db5acef3959efa45b52bc67b61b00823d2a1a6944bf45982 \
+    --hash=sha256:0726c282d188e204281ebd8de31724b7d749adebc086873a59efb8cf7ae27df3 \
+    --hash=sha256:0ceea77719d45c839fd73abcb190b8390412a890df2f83fb8cf49b2a4b5c2f40 \
+    --hash=sha256:114be227f5213ef8b215c22dde19532f5da9652e56e8ce969bf0a26d7c419fee \
+    --hash=sha256:13577ec9e247f8741c84d06b9ece5f654920d8365a4b636ce0e44f15e07ec693 \
+    --hash=sha256:1876b0b653a808fcd50123b953af170c535027bf1d053b59790eebb0aeb38950 \
+    --hash=sha256:1ab0bbcd4d1f7b6991ee7c753655b481c50084294218de69365f8f1970d4c151 \
+    --hash=sha256:1cce488457370ffd1f953846f82323cb6b2ad2190987cd4d70b2713e17268d24 \
+    --hash=sha256:26ee97a8261e6e35885c2ecd2fd4a6d38252246f94a2aec23665a4e66d066305 \
+    --hash=sha256:3528807cbbb7f315bb81959d5961855e7ba52aa60a3097151cb21956fbc7502b \
+    --hash=sha256:374a8e88ddab84b9ada695d255679fb99c53513c0a51778796fcf0944d6c789c \
+    --hash=sha256:376081f471a2ef24828b83a641a02c575d6103a3ad7fd7dade5486cad10ea659 \
+    --hash=sha256:3923a1778f7e5ef31865893fdca12a8d7dc03a44b33e2a5f3295416314c09f5d \
+    --hash=sha256:4916727e31c28be8beaf11cf117d6f6f188dcc36daae4e851fee88646f5b6b18 \
+    --hash=sha256:493c5c5e44b06d6c9268ce21b302c9ca055c1fd3484c25ba41d34476c76ee746 \
+    --hash=sha256:505fe3d03856ac7d215dbe005414bc28505d26f0c128906037e66d98c4e95868 \
+    --hash=sha256:5845fdf5e5d5b78a49b826fcdc0eb2e2aa7191980e3d2cfd2a30303a74f212e2 \
+    --hash=sha256:5c330eace3dd100bdb54b5653b966de7f51c26ec4a7d4e87132d9b4f738220ba \
+    --hash=sha256:5dbf059fb4b7c240c873c1245ee112505be27497e90f7c6591261c7d3c3a8228 \
+    --hash=sha256:5e390971d082dba073c05dbd56322427d3280b7cc8b53484c9377adfbae67dc2 \
+    --hash=sha256:5fbb160554e319f7b22ecf530a80a3ff496d38e8e07ae763b9e82fadfe96f273 \
+    --hash=sha256:64d0fcd436c5683fdd7c907eeae5e2cbb5eb872fafbc03a43609d7941840995c \
+    --hash=sha256:69284049d07fce531c17404fcba2bb1df472bc2dcdac642ae71a2d079d950653 \
+    --hash=sha256:6a0e76621f6e1f908ae52860bdcb58e1ca85231a9b0545e64509c931dd34275a \
+    --hash=sha256:73ee792784d48aa338bba28063e19a27e8d989344f34aad14ea6e1b9bd83f596 \
+    --hash=sha256:74398a4cf19de42e1498368c36eed45d9528f5fd0155241e82c4082b7e16cffd \
+    --hash=sha256:7938111ed1358f536daf311be244f34df7bf3cdedb3ed883787aca97778b28d8 \
+    --hash=sha256:82d92c773fbc6942a7a8b520d22c11cfc8fd83bba86116bfcf962c2f5c2ecdaa \
+    --hash=sha256:83b5c044f3eff2a6534768ccfd50425939e7a8b5cf9a7261c385de1e20dcfc85 \
+    --hash=sha256:8db8e423192303ed77cff4dce3a4b88dbfaf43979d280181558af5e2c3c71afc \
+    --hash=sha256:9517004e21664f2b5a5fd6333b0731b9cf0817403a941b393d89a2f1dc2bd836 \
+    --hash=sha256:95c02b0e27e706e48d0e5426d1710ca78e0f0628d6e89d5b5a5b91a5f12274f3 \
+    --hash=sha256:99881222f4a8c2f641f25703963a5cefb076adffd959e0558dc9f803a52d6a58 \
+    --hash=sha256:9ee32dcb8e531adae1f1ca568822e9b3a738369b3b686d1477cbc643c4a9c128 \
+    --hash=sha256:a22e47578b30a3e199ab067a4d43d790249b3c0587d9a771921f86250c8435db \
+    --hash=sha256:b5505774ea2a73a86ea176e8a9a4a7c8bf5d521050f0f6f8426afe798689243f \
+    --hash=sha256:bd739c9251d01e0279ce729e37b39d49a08c0420d3fee7f2a4968c0576678f77 \
+    --hash=sha256:d16a786905034e7e34098634b184a7d81f91d4c3d246edc6bd7aefb2fd8ea6ad \
+    --hash=sha256:d3420522057ebab1728b21ad473aa950026d07cb09da41103f8e597dfbfaeb13 \
+    --hash=sha256:d56fd9f1f1cdc8227d7b7918f55091349741904d9520c65f0139a9755952c9e8 \
+    --hash=sha256:d661dc4785affa9d0edfdd1e59ec056a58b3dbb9f196fa43587f3ddac654ac7b \
+    --hash=sha256:dfe1f0f0ed5785c187144c46a292b8c34c1295c01da12e10ccddfc16def4448a \
+    --hash=sha256:e1dd7839443592d00e96db831eddb4111a2a81a46b028f0facd60a09ebbdd543 \
+    --hash=sha256:e2872993e209f7ed04d963e4b4fbae72d034844ec66bc4ca403329db2074377b \
+    --hash=sha256:e2f879ab92ce502a1e65fce390eab619774dda6a6ff719718069ac94084098ce \
+    --hash=sha256:e3aa7e51d738e0ec0afbed661261513b38b3014754c9459508399baf14ae0c9d \
+    --hash=sha256:e532dbd6ddfe13946de050d7474e3f5fb6ec774fbb1a188aaf469b08cf04189a \
+    --hash=sha256:e6b7842518a63a9f17107eb176320960ec095a8ee3b4420b5f688e24bf50c53c \
+    --hash=sha256:e75753aeda0ddc4c28dce4c32ba2f6ec30b1b02f6c0b14e547841ba5b24f753f \
+    --hash=sha256:eadb9f826c138e6cf3c49d6f8de88225a3c0ab181a9b4ba792e006e5292d150e \
+    --hash=sha256:ed59dd52075f8fc91da6053b12e8c89e37aa043f8986efd89e61fae69dc1b011 \
+    --hash=sha256:ef254a06bcea461e65ff0373d8a0dd1ed3aa004af48839f002a0c994a6f72d04 \
+    --hash=sha256:f3709997b228685fe53e8c433e2df9f0cdb5f4542bd5114ed17ac3c0129b0480 \
+    --hash=sha256:f51bab98d52739c50c56658cc303f190785f9a2cd97b823357e7aeae54c8f68a \
+    --hash=sha256:f9904e24646570539a8950400602d66d2b2c492b9010ea7e965025cb71d0c86d \
+    --hash=sha256:f9af38a89b6a5c04b7d18c492c8ccf2aee7048aff1ce8437c4683bb5a1df893d
+mypy==1.9.0 \
+    --hash=sha256:0235391f1c6f6ce487b23b9dbd1327b4ec33bb93934aa986efe8a9563d9349e6 \
+    --hash=sha256:190da1ee69b427d7efa8aa0d5e5ccd67a4fb04038c380237a0d96829cb157913 \
+    --hash=sha256:2418488264eb41f69cc64a69a745fad4a8f86649af4b1041a4c64ee61fc61129 \
+    --hash=sha256:3a3c007ff3ee90f69cf0a15cbcdf0995749569b86b6d2f327af01fd1b8aee9dc \
+    --hash=sha256:3cc5da0127e6a478cddd906068496a97a7618a21ce9b54bde5bf7e539c7af974 \
+    --hash=sha256:48533cdd345c3c2e5ef48ba3b0d3880b257b423e7995dada04248725c6f77374 \
+    --hash=sha256:49c87c15aed320de9b438ae7b00c1ac91cd393c1b854c2ce538e2a72d55df150 \
+    --hash=sha256:4d3dbd346cfec7cb98e6cbb6e0f3c23618af826316188d587d1c1bc34f0ede03 \
+    --hash=sha256:571741dc4194b4f82d344b15e8837e8c5fcc462d66d076748142327626a1b6e9 \
+    --hash=sha256:587ce887f75dd9700252a3abbc9c97bbe165a4a630597845c61279cf32dfbf02 \
+    --hash=sha256:5d741d3fc7c4da608764073089e5f58ef6352bedc223ff58f2f038c2c4698a89 \
+    --hash=sha256:5e6061f44f2313b94f920e91b204ec600982961e07a17e0f6cd83371cb23f5c2 \
+    --hash=sha256:61758fabd58ce4b0720ae1e2fea5cfd4431591d6d590b197775329264f86311d \
+    --hash=sha256:653265f9a2784db65bfca694d1edd23093ce49740b2244cde583aeb134c008f3 \
+    --hash=sha256:68edad3dc7d70f2f17ae4c6c1b9471a56138ca22722487eebacfd1eb5321d612 \
+    --hash=sha256:81a10926e5473c5fc3da8abb04119a1f5811a236dc3a38d92015cb1e6ba4cb9e \
+    --hash=sha256:85ca5fcc24f0b4aeedc1d02f93707bccc04733f21d41c88334c5482219b1ccb3 \
+    --hash=sha256:a260627a570559181a9ea5de61ac6297aa5af202f06fd7ab093ce74e7181e43e \
+    --hash=sha256:aceb1db093b04db5cd390821464504111b8ec3e351eb85afd1433490163d60cd \
+    --hash=sha256:b685154e22e4e9199fc95f298661deea28aaede5ae16ccc8cbb1045e716b3e04 \
+    --hash=sha256:d357423fa57a489e8c47b7c85dfb96698caba13d66e086b412298a1a0ea3b0ed \
+    --hash=sha256:d4d5ddc13421ba3e2e082a6c2d74c2ddb3979c39b582dacd53dd5d9431237185 \
+    --hash=sha256:e49499be624dead83927e70c756970a0bc8240e9f769389cdf5714b0784ca6bf \
+    --hash=sha256:e54396d70be04b34f31d2edf3362c1edd023246c82f1730bbf8768c28db5361b \
+    --hash=sha256:f88566144752999351725ac623471661c9d1cd8caa0134ff98cceeea181789f4 \
+    --hash=sha256:f8a67616990062232ee4c3952f41c779afac41405806042a8126fe96e098419f \
+    --hash=sha256:fe28657de3bfec596bbeef01cb219833ad9d38dd5393fc649f4b366840baefe6
 mypy-extensions==1.0.0 \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
-nh3==0.2.15 \
-    --hash=sha256:0d02d0ff79dfd8208ed25a39c12cbda092388fff7f1662466e27d97ad011b770 \
-    --hash=sha256:3277481293b868b2715907310c7be0f1b9d10491d5adf9fce11756a97e97eddf \
-    --hash=sha256:3b803a5875e7234907f7d64777dfde2b93db992376f3d6d7af7f3bc347deb305 \
-    --hash=sha256:427fecbb1031db085eaac9931362adf4a796428ef0163070c484b5a768e71601 \
-    --hash=sha256:5f0d77272ce6d34db6c87b4f894f037d55183d9518f948bba236fe81e2bb4e28 \
-    --hash=sha256:60684857cfa8fdbb74daa867e5cad3f0c9789415aba660614fe16cd66cbb9ec7 \
-    --hash=sha256:6f42f99f0cf6312e470b6c09e04da31f9abaadcd3eb591d7d1a88ea931dca7f3 \
-    --hash=sha256:86e447a63ca0b16318deb62498db4f76fc60699ce0a1231262880b38b6cff911 \
-    --hash=sha256:8d595df02413aa38586c24811237e95937ef18304e108b7e92c890a06793e3bf \
-    --hash=sha256:9c0d415f6b7f2338f93035bba5c0d8c1b464e538bfbb1d598acd47d7969284f0 \
-    --hash=sha256:a5167a6403d19c515217b6bcaaa9be420974a6ac30e0da9e84d4fc67a5d474c5 \
-    --hash=sha256:ac19c0d68cd42ecd7ead91a3a032fdfff23d29302dbb1311e641a130dfefba97 \
-    --hash=sha256:b1e97221cedaf15a54f5243f2c5894bb12ca951ae4ddfd02a9d4ea9df9e1a29d \
-    --hash=sha256:bc2d086fb540d0fa52ce35afaded4ea526b8fc4d3339f783db55c95de40ef02e \
-    --hash=sha256:d1e30ff2d8d58fb2a14961f7aac1bbb1c51f9bdd7da727be35c63826060b0bf3 \
-    --hash=sha256:f3b53ba93bb7725acab1e030bc2ecd012a817040fd7851b332f86e2f9bb98dc6
+nh3==0.2.17 \
+    --hash=sha256:0316c25b76289cf23be6b66c77d3608a4fdf537b35426280032f432f14291b9a \
+    --hash=sha256:1a814dd7bba1cb0aba5bcb9bebcc88fd801b63e21e2450ae6c52d3b3336bc911 \
+    --hash=sha256:1aa52a7def528297f256de0844e8dd680ee279e79583c76d6fa73a978186ddfb \
+    --hash=sha256:22c26e20acbb253a5bdd33d432a326d18508a910e4dcf9a3316179860d53345a \
+    --hash=sha256:40015514022af31975c0b3bca4014634fa13cb5dc4dbcbc00570acc781316dcc \
+    --hash=sha256:40d0741a19c3d645e54efba71cb0d8c475b59135c1e3c580f879ad5514cbf028 \
+    --hash=sha256:551672fd71d06cd828e282abdb810d1be24e1abb7ae2543a8fa36a71c1006fe9 \
+    --hash=sha256:66f17d78826096291bd264f260213d2b3905e3c7fae6dfc5337d49429f1dc9f3 \
+    --hash=sha256:85cdbcca8ef10733bd31f931956f7fbb85145a4d11ab9e6742bbf44d88b7e351 \
+    --hash=sha256:a3f55fabe29164ba6026b5ad5c3151c314d136fd67415a17660b4aaddacf1b10 \
+    --hash=sha256:b4427ef0d2dfdec10b641ed0bdaf17957eb625b2ec0ea9329b3d28806c153d71 \
+    --hash=sha256:ba73a2f8d3a1b966e9cdba7b211779ad8a2561d2dba9674b8a19ed817923f65f \
+    --hash=sha256:c21bac1a7245cbd88c0b0e4a420221b7bfa838a2814ee5bb924e9c2f10a1120b \
+    --hash=sha256:c551eb2a3876e8ff2ac63dff1585236ed5dfec5ffd82216a7a174f7c5082a78a \
+    --hash=sha256:c790769152308421283679a142dbdb3d1c46c79c823008ecea8e8141db1a2062 \
+    --hash=sha256:d7a25fd8c86657f5d9d576268e3b3767c5cd4f42867c9383618be8517f0f022a
 nodeenv==1.8.0 \
     --hash=sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2 \
     --hash=sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec
-packageurl-python==0.13.4 \
-    --hash=sha256:62aa13d60a0082ff115784fefdfe73a12f310e455365cca7c6d362161067f35f \
-    --hash=sha256:6eb5e995009cc73387095e0b507ab65df51357d25ddc5fce3d3545ad6dcbbee8
-packaging==23.2 \
-    --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
-    --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
+packageurl-python==0.15.0 \
+    --hash=sha256:cdc6bd42dc30c4fc7f8f0ccb721fc31f8c33985dbffccb6e6be4c72874de48ca \
+    --hash=sha256:f219b2ce6348185a27bd6a72e6fdc9f984e6c9fa157effa7cb93e341c49cdcc2
+packaging==24.0 \
+    --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
+    --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
 pathspec==0.12.1 \
     --hash=sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08 \
     --hash=sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712
 pbr==6.0.0 \
     --hash=sha256:4a7317d5e3b17a3dccb6a8cfe67dab65b20551404c52c8ed41279fa4f0cb4cda \
     --hash=sha256:d1377122a5a00e2f940ee482999518efe16d745d423a670c27773dfbc3c9a7d9
-pip-api==0.0.30 \
-    --hash=sha256:2a0314bd31522eb9ffe8a99668b0d07fee34ebc537931e7b6483001dbedcbdc9 \
-    --hash=sha256:a05df2c7aa9b7157374bcf4273544201a0c7bae60a9c65bcf84f3959ef3896f3
-pip-audit==2.7.0 \
-    --hash=sha256:67740c5b1d5d967a258c3dfefc46f9713a2819c48062505ddf4b29de101c2b75 \
-    --hash=sha256:83e039740653eb9ef1a78b1540ed441600cd88a560588ba2c0a169180685a522
+pip-api==0.0.33 \
+    --hash=sha256:1c2522ae21efcb034d89cc99f6cf1025293b31c63c29ee98b23f03a85f36bdae \
+    --hash=sha256:b8d6eb5a87d3a9e112a20a8e9d24a6fc12d4e1c94d7595eeaf74be11ad47276c
+pip-audit==2.7.2 \
+    --hash=sha256:49907430115baacb8bb7ffc1a2b689acfeac9d8534a43bffad3c73f8d8b32d52 \
+    --hash=sha256:a12905e42dd452f43a2dbf895606d59c35348deed27b8cbaff8516423576fdfb
 pip-requirements-parser==32.0.1 \
     --hash=sha256:4659bc2a667783e7a15d190f6fccf8b2486685b6dba4c19c3876314769c57526 \
     --hash=sha256:b4fa3a7a0be38243123cf9d1f3518da10c51bdb165a2b2985566247f9155a7d3
-pip-tools==7.3.0 \
-    --hash=sha256:8717693288720a8c6ebd07149c93ab0be1fced0b5191df9e9decd3263e20d85e \
-    --hash=sha256:8e9c99127fe024c025b46a0b2d15c7bd47f18f33226cf7330d35493663fc1d1d
-pkginfo==1.9.6 \
-    --hash=sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546 \
-    --hash=sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046
-platformdirs==4.1.0 \
-    --hash=sha256:11c8f37bcca40db96d8144522d925583bdb7a31f7b0e37e3ed4318400a8e2380 \
-    --hash=sha256:906d548203468492d432bcb294d4bc2fff751bf84971fbb2c10918cc206ee420
+pip-tools==7.4.1 \
+    --hash=sha256:4c690e5fbae2f21e87843e89c26191f0d9454f362d8acdbd695716493ec8b3a9 \
+    --hash=sha256:864826f5073864450e24dbeeb85ce3920cdfb09848a3d69ebf537b521f14bcc9
+pkginfo==1.10.0 \
+    --hash=sha256:5df73835398d10db79f8eecd5cd86b1f6d29317589ea70796994d49399af6297 \
+    --hash=sha256:889a6da2ed7ffc58ab5b900d888ddce90bce912f2d2de1dc1c26f4cb9fe65097
+platformdirs==4.2.0 \
+    --hash=sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068 \
+    --hash=sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768
 pluggy==1.4.0 \
     --hash=sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981 \
     --hash=sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be
-pre-commit==3.6.0 \
-    --hash=sha256:c255039ef399049a5544b6ce13d135caba8f2c28c3b4033277a788f434308376 \
-    --hash=sha256:d30bad9abf165f7785c15a21a1f46da7d0677cb00ee7ff4c579fd38922efe15d
-py-serializable==1.0.0 \
-    --hash=sha256:524df68c46315d7272959ae5296244e5a1e1e28330472ec214394162c39f545e \
-    --hash=sha256:845a9399a16550e8703c3fb0da4fbb746a4e5f6cc4c95647c315c71fd6567cd5
+pre-commit==3.7.0 \
+    --hash=sha256:5eae9e10c2b5ac51577c3452ec0a490455c45a0533f7960f993a0d01e59decab \
+    --hash=sha256:e209d61b8acdcf742404408531f0c37d49d2c734fd7cff2d6076083d191cb060
+py-serializable==1.0.3 \
+    --hash=sha256:afba815f465b9fe7ab1c1a56d1aa8880c8a9e67a6e28b7ed62d4696fa369caf8 \
+    --hash=sha256:da3cb4b1f3cc5cc5ebecdd3dadbabd5f65d764357366fa64ee9cbaf0d4b70dcf
 pycodestyle==2.11.1 \
     --hash=sha256:41ba0e7afc9752dfb53ced5489e89f8186be00e599e712660695b7a75ff2663f \
     --hash=sha256:44fe31000b2d866f2e41841b18528a505fbd7fef9017b04eff4e2648a0fadc67
-pycparser==2.21 \
-    --hash=sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9 \
-    --hash=sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206
+pycparser==2.22 \
+    --hash=sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6 \
+    --hash=sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc
 pyflakes==3.2.0 \
     --hash=sha256:1c61603ff154621fb2a9172037d84dca3500def8c8b630657d1701f026f8af3f \
     --hash=sha256:84b5be138a2dfbb40689ca07e2152deb896a65c3a3e24c251c5c62489568074a
 pygments==2.17.2 \
     --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
     --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
-pylint==3.0.3 \
-    --hash=sha256:58c2398b0301e049609a8429789ec6edf3aabe9b6c5fec916acd18639c16de8b \
-    --hash=sha256:7a1585285aefc5165db81083c3e06363a27448f6b467b3b0f30dbd0ac1f73810
-pyparsing==3.1.1 \
-    --hash=sha256:32c7c0b711493c72ff18a981d24f28aaf9c1fb7ed5e9667c9e84e3db623bdbfb \
-    --hash=sha256:ede28a1a32462f5a9705e07aea48001a08f7cf81a021585011deba701581a0db
+pylint==3.1.0 \
+    --hash=sha256:507a5b60953874766d8a366e8e8c7af63e058b26345cfcb5f91f89d987fd6b74 \
+    --hash=sha256:6a69beb4a6f63debebaab0a3477ecd0f559aa726af4954fc948c51f7a2549e23
+pyparsing==3.1.2 \
+    --hash=sha256:a1bac0ce561155ecc3ed78ca94d3c9378656ad4c94c1270de543f621420f94ad \
+    --hash=sha256:f9db75911801ed778fe61bb643079ff86601aca99fcae6345aa67292038fb742
 pyproject-hooks==1.0.0 \
     --hash=sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8 \
     --hash=sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5
-pytest==8.0.0 \
-    --hash=sha256:249b1b0864530ba251b7438274c4d251c58d868edaaec8762893ad4a0d71c36c \
-    --hash=sha256:50fb9cbe836c3f20f0dfa99c565201fb75dc54c8d76373cd1bde06b06657bdb6
-pytest-cov==4.1.0 \
-    --hash=sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6 \
-    --hash=sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a
+pytest==8.1.1 \
+    --hash=sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7 \
+    --hash=sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044
+pytest-cov==5.0.0 \
+    --hash=sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652 \
+    --hash=sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857
 pytest-env==1.1.3 \
     --hash=sha256:aada77e6d09fcfb04540a6e462c58533c37df35fa853da78707b17ec04d17dfc \
     --hash=sha256:fcd7dc23bb71efd3d35632bde1bbe5ee8c8dc4489d6617fb010674880d96216b
-python-dateutil==2.8.2 \
-    --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
-    --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
-python-slugify==8.0.2 \
-    --hash=sha256:428ea9b00c977b8f6c097724398f190b2c18e2a6011094d1001285875ccacdbf \
-    --hash=sha256:a1a02b127a95c124fd84f8f88be730e557fd823774bf19b1cd5e8704e2ae0e5e
-pyupgrade==3.15.0 \
-    --hash=sha256:8dc8ebfaed43566e2c65994162795017c7db11f531558a74bc8aa077907bc305 \
-    --hash=sha256:a7fde381060d7c224f55aef7a30fae5ac93bbc428367d27e70a603bc2acd4f00
+python-dateutil==2.9.0.post0 \
+    --hash=sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3 \
+    --hash=sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427
+python-slugify==8.0.4 \
+    --hash=sha256:276540b79961052b66b7d116620b36518847f52d5fd9e3a70164fc8c50faa6b8 \
+    --hash=sha256:59202371d1d05b54a9e7720c5e038f928f45daaffe41dd10822f3907b937c856
+pyupgrade==3.15.2 \
+    --hash=sha256:c488d6896c546d25845712ef6402657123008d56c1063174e27aabe15bd6b4e5 \
+    --hash=sha256:ce309e0ff8ecb73f56a45f12570be84bbbde9540d13697cacb261a7f595fb1f5
 pyyaml==6.0.1 \
     --hash=sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5 \
     --hash=sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc \
     --hash=sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df \
     --hash=sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741 \
     --hash=sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206 \
     --hash=sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27 \
@@ -657,80 +666,80 @@
     --hash=sha256:e7d73685e87afe9f3b36c799222440d6cf362062f78be1013661b00c5c6f678b \
     --hash=sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab \
     --hash=sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa \
     --hash=sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c \
     --hash=sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585 \
     --hash=sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d \
     --hash=sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f
-readme-renderer==42.0 \
-    --hash=sha256:13d039515c1f24de668e2c93f2e877b9dbe6c6c32328b90a40a49d8b2b85f36d \
-    --hash=sha256:2d55489f83be4992fe4454939d1a051c33edbab778e82761d060c9fc6b308cd1
+readme-renderer==43.0 \
+    --hash=sha256:1818dd28140813509eeed8d62687f7cd4f7bad90d4db586001c5dc09d4fde311 \
+    --hash=sha256:19db308d86ecd60e5affa3b2a98f017af384678c63c88e5d4556a380e674f3f9
 requests==2.31.0 \
     --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
     --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
 requests-toolbelt==1.0.0 \
     --hash=sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6 \
     --hash=sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06
 rfc3986==2.0.0 \
     --hash=sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd \
     --hash=sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c
-rich==13.7.0 \
-    --hash=sha256:5cb5123b5cf9ee70584244246816e9114227e0b98ad9176eede6ad54bf5403fa \
-    --hash=sha256:6da14c108c4866ee9520bbffa71f6fe3962e193b7da68720583850cd4548e235
+rich==13.7.1 \
+    --hash=sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222 \
+    --hash=sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432
 secretstorage==3.3.3 \
     --hash=sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77 \
     --hash=sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99
 six==1.16.0 \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
 sortedcontainers==2.4.0 \
     --hash=sha256:25caa5a06cc30b6b83d11423433f65d1f9d76c4c6a0c90e3379eaa43b9bfdb88 \
     --hash=sha256:a163dcaede0f1c021485e957a39245190e74249897e2ae4b2aa38595db237ee0
-stevedore==5.1.0 \
-    --hash=sha256:8cc040628f3cea5d7128f2e76cf486b2251a4e543c7b938f58d9a377f6694a2d \
-    --hash=sha256:a54534acf9b89bc7ed264807013b505bf07f74dbe4bcfa37d32bd063870b087c
+stevedore==5.2.0 \
+    --hash=sha256:1c15d95766ca0569cad14cb6272d4d31dae66b011a929d7c18219c176ea1b5c9 \
+    --hash=sha256:46b93ca40e1114cea93d738a6c1e365396981bb6bb78c27045b7587c9473544d
 text-unidecode==1.3 \
     --hash=sha256:1311f10e8b895935241623731c2ba64f4c455287888b18189350b67134a822e8 \
     --hash=sha256:bad6603bb14d279193107714b288be206cac565dfa49aa5b105294dd5c4aab93
 tokenize-rt==5.2.0 \
     --hash=sha256:9fe80f8a5c1edad2d3ede0f37481cc0cc1538a2f442c9c2f9e4feacd2792d054 \
     --hash=sha256:b79d41a65cfec71285433511b50271b05da3584a1da144a0752e9c621a285289
 toml==0.10.2 \
     --hash=sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b \
     --hash=sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f
-tomlkit==0.12.3 \
-    --hash=sha256:75baf5012d06501f07bee5bf8e801b9f343e7aac5a92581f20f80ce632e6b5a4 \
-    --hash=sha256:b0a645a9156dc7cb5d3a1f0d4bab66db287fcb8e0430bdd4664a095ea16414ba
-twine==4.0.2 \
-    --hash=sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8 \
-    --hash=sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8
-types-python-dateutil==2.8.19.20240106 \
-    --hash=sha256:1f8db221c3b98e6ca02ea83a58371b22c374f42ae5bbdf186db9c9a76581459f \
-    --hash=sha256:efbbdc54590d0f16152fa103c9879c7d4a00e82078f6e2cf01769042165acaa2
-typing-extensions==4.9.0 \
-    --hash=sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783 \
-    --hash=sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd
+tomlkit==0.12.4 \
+    --hash=sha256:5cd82d48a3dd89dee1f9d64420aa20ae65cfbd00668d6f094d7578a78efbb77b \
+    --hash=sha256:7ca1cfc12232806517a8515047ba66a19369e71edf2439d0f5824f91032b6cc3
+twine==5.0.0 \
+    --hash=sha256:89b0cc7d370a4b66421cc6102f269aa910fe0f1861c124f573cf2ddedbc10cf4 \
+    --hash=sha256:a262933de0b484c53408f9edae2e7821c1c45a3314ff2df9bdd343aa7ab8edc0
+types-python-dateutil==2.9.0.20240316 \
+    --hash=sha256:5d2f2e240b86905e40944dd787db6da9263f0deabef1076ddaed797351ec0202 \
+    --hash=sha256:6b8cb66d960771ce5ff974e9dd45e38facb81718cc1e208b10b1baccbfdbee3b
+typing-extensions==4.11.0 \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
 untokenize==0.1.1 \
     --hash=sha256:3865dbbbb8efb4bb5eaa72f1be7f3e0be00ea8b7f125c69cbd1f5fda926f37a2
-urllib3==2.1.0 \
-    --hash=sha256:55901e917a5896a349ff771be919f8bd99aff50b79fe58fec595eb37bbc56bb3 \
-    --hash=sha256:df7aa8afb0148fa78488e7899b2c59b5f4ffcfa82e6c54ccb9dd37c1d7b52d54
-virtualenv==20.25.0 \
-    --hash=sha256:4238949c5ffe6876362d9c0180fc6c3a824a7b12b80604eeb8085f2ed7460de3 \
-    --hash=sha256:bf51c0d9c7dd63ea8e44086fa1e4fb1093a31e963b86959257378aef020e1f1b
+urllib3==2.2.1 \
+    --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
+    --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
+virtualenv==20.25.1 \
+    --hash=sha256:961c026ac520bac5f69acb8ea063e8a4f071bcc9457b9c1f28f6b085c511583a \
+    --hash=sha256:e08e13ecdca7a0bd53798f356d5831434afa5b07b93f0abdf0797b7a06ffe197
 webencodings==0.5.1 \
     --hash=sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78 \
     --hash=sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923
-wheel==0.42.0 \
-    --hash=sha256:177f9c9b0d45c47873b619f5b650346d632cdc35fb5e4d25058e09c9e581433d \
-    --hash=sha256:c45be39f7882c9d34243236f2d63cbd58039e360f85d0913425fbd7ceea617a8
-zipp==3.17.0 \
-    --hash=sha256:0e923e726174922dce09c53c59ad483ff7bbb8e572e00c7f7c46b88556409f31 \
-    --hash=sha256:84e64a1c28cf7e91ed2078bb8cc8c259cb19b76942096c8d7b84947690cabaf0
+wheel==0.43.0 \
+    --hash=sha256:465ef92c69fa5c5da2d1cf8ac40559a8c940886afcef87dcf14b9470862f1d85 \
+    --hash=sha256:55c570405f142630c6b9f72fe09d9b67cf1477fcf543ae5b8dcb1f5b7377da81
+zipp==3.18.1 \
+    --hash=sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b \
+    --hash=sha256:2884ed22e7d8961de1c9a05142eb69a247f120291bc0206a00a7642f09b5b715
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==23.3.2 \
-    --hash=sha256:5052d7889c1f9d05224cd41741acb7c5d6fa735ab34e339624a614eaaa7e7d76 \
-    --hash=sha256:7fd9972f96db22c8077a1ee2691b172c8089b17a5652a44494a9ecb0d78f9149
-setuptools==69.0.3 \
-    --hash=sha256:385eb4edd9c9d5c17540511303e39a147ce2fc04bc55289c322b9e5904fe2c05 \
-    --hash=sha256:be1af57fc409f93647f2e8e4573a142ed38724b8cdd389706a867bb4efcf1e78
+pip==24.0 \
+    --hash=sha256:ba0d021a166865d2265246961bec0152ff124de910c5cc39f1156ce3fa7c69dc \
+    --hash=sha256:ea9bd1a847e8c5774a5777bb398c19e80bcd4e2aa16a4b301b718fe6f593aba2
+setuptools==69.2.0 \
+    --hash=sha256:0ff4183f8f42cd8fa3acea16c45205521a4ef28f73c6391d8a25e92893134f2e \
+    --hash=sha256:c21c49fb1042386df081cb5d86759792ab89efca84cf114889191cd09aacc80c
```

### Comparing `cookiecutter-python-vscode-github-0.6.0/tests/test_main.py` & `cookiecutter_python_vscode_github-0.7.0/tests/test_main.py`

 * *Files identical despite different names*

