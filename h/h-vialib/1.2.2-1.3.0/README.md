# Comparing `tmp/h-vialib-1.2.2.tar.gz` & `tmp/h_vialib-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h-vialib-1.2.2.tar", last modified: Wed Feb 28 08:39:48 2024, max compression
+gzip compressed data, was "h_vialib-1.3.0.tar", last modified: Thu May  2 10:00:32 2024, max compression
```

## Comparing `h-vialib-1.2.2.tar` & `h_vialib-1.3.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.856120 h-vialib-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.848121 h-vialib-1.2.2/.cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-02-28 08:39:42.000000 h-vialib-1.2.2/.cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.844121 h-vialib-1.2.2/.cookiecutter/includes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.848121 h-vialib-1.2.2/.cookiecutter/includes/README/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-28 08:39:42.000000 h-vialib-1.2.2/.cookiecutter/includes/README/head.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.848121 h-vialib-1.2.2/.cookiecutter/includes/setuptools/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-28 08:39:42.000000 h-vialib-1.2.2/.cookiecutter/includes/setuptools/install_requires
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.848121 h-vialib-1.2.2/.cookiecutter/includes/tox/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-28 08:39:42.000000 h-vialib-1.2.2/.cookiecutter/includes/tox/deps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.848121 h-vialib-1.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-28 08:39:42.000000 h-vialib-1.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.852120 h-vialib-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-02-28 08:39:42.000000 h-vialib-1.2.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-28 08:39:42.000000 h-vialib-1.2.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-02-28 08:39:42.000000 h-vialib-1.2.2/.github/workflows/slack.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-28 08:39:42.000000 h-vialib-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-28 08:39:42.000000 h-vialib-1.2.2/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-02-28 08:39:42.000000 h-vialib-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-02-28 08:39:42.000000 h-vialib-1.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-02-28 08:39:48.856120 h-vialib-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-02-28 08:39:42.000000 h-vialib-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.852120 h-vialib-1.2.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      527 2024-02-28 08:39:42.000000 h-vialib-1.2.2/bin/make_python
--rwxr-xr-x   0 runner    (1001) docker     (127)     1372 2024-02-28 08:39:42.000000 h-vialib-1.2.2/bin/make_template
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-02-28 08:39:42.000000 h-vialib-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-28 08:39:48.856120 h-vialib-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.848121 h-vialib-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.852120 h-vialib-1.2.2/src/h_vialib/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-02-28 08:39:42.000000 h-vialib-1.2.2/src/h_vialib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-02-28 08:39:42.000000 h-vialib-1.2.2/src/h_vialib/_flat_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-02-28 08:39:42.000000 h-vialib-1.2.2/src/h_vialib/_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-02-28 08:39:42.000000 h-vialib-1.2.2/src/h_vialib/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-02-28 08:39:42.000000 h-vialib-1.2.2/src/h_vialib/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-28 08:39:42.000000 h-vialib-1.2.2/src/h_vialib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.852120 h-vialib-1.2.2/src/h_vialib/secure/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-28 08:39:42.000000 h-vialib-1.2.2/src/h_vialib/secure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-02-28 08:39:42.000000 h-vialib-1.2.2/src/h_vialib/secure/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-02-28 08:39:42.000000 h-vialib-1.2.2/src/h_vialib/secure/expiry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-02-28 08:39:42.000000 h-vialib-1.2.2/src/h_vialib/secure/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-02-28 08:39:42.000000 h-vialib-1.2.2/src/h_vialib/secure/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.856120 h-vialib-1.2.2/src/h_vialib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-02-28 08:39:48.000000 h-vialib-1.2.2/src/h_vialib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-02-28 08:39:48.000000 h-vialib-1.2.2/src/h_vialib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 08:39:48.000000 h-vialib-1.2.2/src/h_vialib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-28 08:39:48.000000 h-vialib-1.2.2/src/h_vialib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-28 08:39:48.000000 h-vialib-1.2.2/src/h_vialib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.852120 h-vialib-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.852120 h-vialib-1.2.2/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tests/functional/sanity_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tests/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.856120 h-vialib-1.2.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.856120 h-vialib-1.2.2/tests/unit/h_vialib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tests/unit/h_vialib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tests/unit/h_vialib/_flat_dict_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tests/unit/h_vialib/_params_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tests/unit/h_vialib/client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tests/unit/h_vialib/configuration_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:48.856120 h-vialib-1.2.2/tests/unit/h_vialib/secure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tests/unit/h_vialib/secure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tests/unit/h_vialib/secure/encryption_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tests/unit/h_vialib/secure/expiry_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tests/unit/h_vialib/secure/token_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tests/unit/h_vialib/secure/url_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-02-28 08:39:42.000000 h-vialib-1.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.640817 h_vialib-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.636817 h_vialib-1.3.0/.cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-02 10:00:26.000000 h_vialib-1.3.0/.cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.632817 h_vialib-1.3.0/.cookiecutter/includes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.636817 h_vialib-1.3.0/.cookiecutter/includes/README/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-02 10:00:26.000000 h_vialib-1.3.0/.cookiecutter/includes/README/head.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.636817 h_vialib-1.3.0/.cookiecutter/includes/setuptools/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 10:00:26.000000 h_vialib-1.3.0/.cookiecutter/includes/setuptools/install_requires
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.636817 h_vialib-1.3.0/.cookiecutter/includes/tox/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 10:00:26.000000 h_vialib-1.3.0/.cookiecutter/includes/tox/deps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.636817 h_vialib-1.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-02 10:00:26.000000 h_vialib-1.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.636817 h_vialib-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-02 10:00:26.000000 h_vialib-1.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-02 10:00:26.000000 h_vialib-1.3.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-02 10:00:26.000000 h_vialib-1.3.0/.github/workflows/slack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-02 10:00:26.000000 h_vialib-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-02 10:00:26.000000 h_vialib-1.3.0/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-02 10:00:26.000000 h_vialib-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-02 10:00:26.000000 h_vialib-1.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-02 10:00:32.640817 h_vialib-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-02 10:00:26.000000 h_vialib-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.636817 h_vialib-1.3.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      527 2024-05-02 10:00:26.000000 h_vialib-1.3.0/bin/make_python
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1372 2024-05-02 10:00:26.000000 h_vialib-1.3.0/bin/make_template
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-02 10:00:26.000000 h_vialib-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-02 10:00:32.640817 h_vialib-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.632817 h_vialib-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.636817 h_vialib-1.3.0/src/h_vialib/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 10:00:26.000000 h_vialib-1.3.0/src/h_vialib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-02 10:00:26.000000 h_vialib-1.3.0/src/h_vialib/_flat_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-02 10:00:26.000000 h_vialib-1.3.0/src/h_vialib/_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-02 10:00:26.000000 h_vialib-1.3.0/src/h_vialib/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-05-02 10:00:26.000000 h_vialib-1.3.0/src/h_vialib/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-02 10:00:26.000000 h_vialib-1.3.0/src/h_vialib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.640817 h_vialib-1.3.0/src/h_vialib/secure/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 10:00:26.000000 h_vialib-1.3.0/src/h_vialib/secure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-02 10:00:26.000000 h_vialib-1.3.0/src/h_vialib/secure/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-02 10:00:26.000000 h_vialib-1.3.0/src/h_vialib/secure/expiry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-02 10:00:26.000000 h_vialib-1.3.0/src/h_vialib/secure/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-02 10:00:26.000000 h_vialib-1.3.0/src/h_vialib/secure/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.640817 h_vialib-1.3.0/src/h_vialib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-02 10:00:32.000000 h_vialib-1.3.0/src/h_vialib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-02 10:00:32.000000 h_vialib-1.3.0/src/h_vialib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:00:32.000000 h_vialib-1.3.0/src/h_vialib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-02 10:00:32.000000 h_vialib-1.3.0/src/h_vialib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 10:00:32.000000 h_vialib-1.3.0/src/h_vialib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.640817 h_vialib-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.640817 h_vialib-1.3.0/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tests/functional/sanity_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tests/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.640817 h_vialib-1.3.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.640817 h_vialib-1.3.0/tests/unit/h_vialib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tests/unit/h_vialib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tests/unit/h_vialib/_flat_dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tests/unit/h_vialib/_params_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tests/unit/h_vialib/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tests/unit/h_vialib/configuration_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:32.640817 h_vialib-1.3.0/tests/unit/h_vialib/secure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tests/unit/h_vialib/secure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tests/unit/h_vialib/secure/encryption_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tests/unit/h_vialib/secure/expiry_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tests/unit/h_vialib/secure/token_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tests/unit/h_vialib/secure/url_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-02 10:00:26.000000 h_vialib-1.3.0/tox.ini
```

### Comparing `h-vialib-1.2.2/.cookiecutter/cookiecutter.json` & `h_vialib-1.3.0/.cookiecutter/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/.github/workflows/ci.yml` & `h_vialib-1.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/.github/workflows/slack.yml` & `h_vialib-1.3.0/.github/workflows/slack.yml`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/LICENSE` & `h_vialib-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/Makefile` & `h_vialib-1.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/PKG-INFO` & `h_vialib-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: h-vialib
-Version: 1.2.2
+Version: 1.3.0
 Summary: Library functions for use with Via.
 Home-page: https://github.com/hypothesis/h-vialib
 Project-URL: Bug Tracker, https://github.com/hypothesis/h-vialib/issues
 Project-URL: Changelog, https://github.com/hypothesis/h-vialib/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: python-jose[cryptography]
+Requires-Dist: joserfc
 Requires-Dist: webob
 
 <a href="https://github.com/hypothesis/h-vialib/actions/workflows/ci.yml?query=branch%3Amain"><img src="https://img.shields.io/github/actions/workflow/status/hypothesis/h-vialib/ci.yml?branch=main"></a>
 <a href="https://pypi.org/project/h-vialib"><img src="https://img.shields.io/pypi/v/h-vialib"></a>
 <a><img src="https://img.shields.io/badge/python-3.9 | 3.8-success"></a>
 <a href="https://github.com/hypothesis/h-vialib/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-BSD--2--Clause-success"></a>
 <a href="https://github.com/hypothesis/cookiecutters/tree/main/pypackage"><img src="https://img.shields.io/badge/cookiecutter-pypackage-success"></a>
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: h-vialib Version: 1.2.2 Summary: Library functions
+Metadata-Version: 2.1 Name: h-vialib Version: 1.3.0 Summary: Library functions
 for use with Via. Home-page: https://github.com/hypothesis/h-vialib Project-
 URL: Bug Tracker, https://github.com/hypothesis/h-vialib/issues Project-URL:
 Changelog, https://github.com/hypothesis/h-vialib/releases Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: BSD
 License Classifier: Intended Audience :: Developers Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-python-jose[cryptography] Requires-Dist: webob _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
-_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_h_y_p_o_t_h_e_s_i_s_/_h_-_v_i_a_l_i_b_/_c_i_._y_m_l_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_h_-_v_i_a_l_i_b_][https://img.shields.io/badge/python-3.9 | 3.8-
-success]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_l_i_c_e_n_s_e_-_B_S_D_-_-_2_-_-_C_l_a_u_s_e_-_s_u_c_c_e_s_s_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_o_k_i_e_c_u_t_t_e_r_-_p_y_p_a_c_k_a_g_e_-_s_u_c_c_e_s_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_]# h-vialib Library functions for use with Via.
-Usage ----- This is an internal library, mostly of interest to maintainers of
-[Via](https://github.com/hypothesis/via) and related components. Some items of
+joserfc Requires-Dist: webob _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/
+_s_t_a_t_u_s_/_h_y_p_o_t_h_e_s_i_s_/_h_-_v_i_a_l_i_b_/_c_i_._y_m_l_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_h_-
+_v_i_a_l_i_b_][https://img.shields.io/badge/python-3.9 | 3.8-success]_[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_l_i_c_e_n_s_e_-_B_S_D_-_-_2_-_-_C_l_a_u_s_e_-_s_u_c_c_e_s_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_b_a_d_g_e_/_c_o_o_k_i_e_c_u_t_t_e_r_-_p_y_p_a_c_k_a_g_e_-_s_u_c_c_e_s_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
+_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_]# h-vialib Library functions for use with Via. Usage
+----- This is an internal library, mostly of interest to maintainers of [Via]
+(https://github.com/hypothesis/via) and related components. Some items of
 interest: * [Configuration](https://github.com/hypothesis/h-vialib/blob/main/
 src/h_vialib/configuration.py) - Configuration parameter management ## Setting
 up Your h-vialib Development Environment First you'll need to install: * [Git]
 (https://git-scm.com/). On Ubuntu: `sudo apt install git`, on macOS: `brew
 install git`. * [GNU Make](https://www.gnu.org/software/make/). This is
 probably already installed, run `make --version` to check. * [pyenv](https://
 github.com/pyenv/pyenv). Follow the instructions in pyenv's README to install
```

### Comparing `h-vialib-1.2.2/README.md` & `h_vialib-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/bin/make_python` & `h_vialib-1.3.0/bin/make_python`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/bin/make_template` & `h_vialib-1.3.0/bin/make_template`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/pyproject.toml` & `h_vialib-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/setup.cfg` & `h_vialib-1.3.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	python-jose[cryptography]
+	joserfc
 	webob
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
```

### Comparing `h-vialib-1.2.2/src/h_vialib/_flat_dict.py` & `h_vialib-1.3.0/src/h_vialib/_flat_dict.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/src/h_vialib/_params.py` & `h_vialib-1.3.0/src/h_vialib/_params.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/src/h_vialib/client.py` & `h_vialib-1.3.0/src/h_vialib/client.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/src/h_vialib/configuration.py` & `h_vialib-1.3.0/src/h_vialib/configuration.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/src/h_vialib/secure/encryption.py` & `h_vialib-1.3.0/src/h_vialib/secure/encryption.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import json
 
-from jose import constants, jwe
+from joserfc import jwe
 
 
 class Encryption:
-    JWE_ALGORITHM = constants.ALGORITHMS.DIR
-    JWE_ENCRYPTION = constants.ALGORITHMS.A128CBC_HS256
+    JWE_ALGORITHM = "dir"
+    JWE_ENCRYPTION = "A128CBC-HS256"
 
     def __init__(self, secret: bytes):
         self._secret = secret.ljust(32)[:32]
 
     def encrypt_dict(self, payload: dict) -> str:
         """Encrypt a dictionary as a JWE."""
-
-        return jwe.encrypt(
-            json.dumps(payload),
-            self._secret,
-            algorithm=self.JWE_ALGORITHM,
-            encryption=self.JWE_ENCRYPTION,
-        ).decode("utf-8")
+        protected = {"alg": self.JWE_ALGORITHM, "enc": self.JWE_ENCRYPTION}
+        return jwe.encrypt_compact(
+            protected, json.dumps(payload).encode("utf-8"), self._secret
+        )
 
     def decrypt_dict(self, payload: str) -> dict:
         """Decrypts payloads created by `encrypt_dict`."""
-
-        return json.loads(jwe.decrypt(payload, self._secret))
+        data = jwe.decrypt_compact(payload, self._secret).plaintext
+        return json.loads(data)
```

### Comparing `h-vialib-1.2.2/src/h_vialib/secure/expiry.py` & `h_vialib-1.3.0/src/h_vialib/secure/expiry.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/src/h_vialib/secure/token.py` & `h_vialib-1.3.0/src/h_vialib/secure/token.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """JWT based tokens which can be used to create verifiable, expiring tokens."""
 
-from jose import jwt
-from jose.exceptions import ExpiredSignatureError, JWTError
+from joserfc import jwt
+from joserfc.errors import JoseError
 
 from h_vialib.exceptions import InvalidToken, MissingToken
 from h_vialib.secure.expiry import as_expires
 
 
 class SecureToken:
     """A standardized and simplified JWT token."""
@@ -15,39 +15,39 @@
     def __init__(self, secret):
         """Initialise a token creator.
 
         :param secret: The secret to sign and check tokens with
         """
         self._secret = secret
 
-    def create(self, payload=None, expires=None, max_age=None):
+    def create(self, payload=None, expires=None, max_age=None) -> str:
         """Create a secure token.
 
         :param payload: Dict of information to put in the token
         :param expires: Datetime by which this token with expire
         :param max_age: ... or max age in seconds after which this will expire
         :return: A JWT encoded token as a string
 
         :raise ValueError: if neither expires nor max_age is specified
         """
-        payload["exp"] = as_expires(expires, max_age)
+        payload["exp"] = int(as_expires(expires, max_age).timestamp())
+        return jwt.encode({"alg": self.TOKEN_ALGORITHM}, payload, self._secret)
 
-        return jwt.encode(payload, self._secret, self.TOKEN_ALGORITHM)
-
-    def verify(self, token):
+    def verify(self, token: str) -> dict:
         """Decode a token and check for validity.
 
         :param token: Token string to check
         :return: The token payload if valid
 
         :raise InvalidToken: If the token is invalid or expired
         :raise MissingToken: If no token is provided
         """
         if not token:
             raise MissingToken("Missing secure token")
 
         try:
-            return jwt.decode(token, self._secret, self.TOKEN_ALGORITHM)
-        except ExpiredSignatureError as err:
-            raise InvalidToken("Expired secure token") from err
-        except JWTError as err:
-            raise InvalidToken("Invalid secure token") from err
+            claims = jwt.decode(token, self._secret).claims
+            jwt.JWTClaimsRegistry().validate(claims)
+        except JoseError as err:
+            raise InvalidToken() from err
+
+        return claims
```

### Comparing `h-vialib-1.2.2/src/h_vialib/secure/url.py` & `h_vialib-1.3.0/src/h_vialib/secure/url.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/src/h_vialib.egg-info/PKG-INFO` & `h_vialib-1.3.0/src/h_vialib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: h-vialib
-Version: 1.2.2
+Version: 1.3.0
 Summary: Library functions for use with Via.
 Home-page: https://github.com/hypothesis/h-vialib
 Project-URL: Bug Tracker, https://github.com/hypothesis/h-vialib/issues
 Project-URL: Changelog, https://github.com/hypothesis/h-vialib/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: python-jose[cryptography]
+Requires-Dist: joserfc
 Requires-Dist: webob
 
 <a href="https://github.com/hypothesis/h-vialib/actions/workflows/ci.yml?query=branch%3Amain"><img src="https://img.shields.io/github/actions/workflow/status/hypothesis/h-vialib/ci.yml?branch=main"></a>
 <a href="https://pypi.org/project/h-vialib"><img src="https://img.shields.io/pypi/v/h-vialib"></a>
 <a><img src="https://img.shields.io/badge/python-3.9 | 3.8-success"></a>
 <a href="https://github.com/hypothesis/h-vialib/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-BSD--2--Clause-success"></a>
 <a href="https://github.com/hypothesis/cookiecutters/tree/main/pypackage"><img src="https://img.shields.io/badge/cookiecutter-pypackage-success"></a>
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: h-vialib Version: 1.2.2 Summary: Library functions
+Metadata-Version: 2.1 Name: h-vialib Version: 1.3.0 Summary: Library functions
 for use with Via. Home-page: https://github.com/hypothesis/h-vialib Project-
 URL: Bug Tracker, https://github.com/hypothesis/h-vialib/issues Project-URL:
 Changelog, https://github.com/hypothesis/h-vialib/releases Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: BSD
 License Classifier: Intended Audience :: Developers Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-python-jose[cryptography] Requires-Dist: webob _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
-_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_h_y_p_o_t_h_e_s_i_s_/_h_-_v_i_a_l_i_b_/_c_i_._y_m_l_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_h_-_v_i_a_l_i_b_][https://img.shields.io/badge/python-3.9 | 3.8-
-success]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_l_i_c_e_n_s_e_-_B_S_D_-_-_2_-_-_C_l_a_u_s_e_-_s_u_c_c_e_s_s_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_o_k_i_e_c_u_t_t_e_r_-_p_y_p_a_c_k_a_g_e_-_s_u_c_c_e_s_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_]# h-vialib Library functions for use with Via.
-Usage ----- This is an internal library, mostly of interest to maintainers of
-[Via](https://github.com/hypothesis/via) and related components. Some items of
+joserfc Requires-Dist: webob _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/
+_s_t_a_t_u_s_/_h_y_p_o_t_h_e_s_i_s_/_h_-_v_i_a_l_i_b_/_c_i_._y_m_l_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_h_-
+_v_i_a_l_i_b_][https://img.shields.io/badge/python-3.9 | 3.8-success]_[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_l_i_c_e_n_s_e_-_B_S_D_-_-_2_-_-_C_l_a_u_s_e_-_s_u_c_c_e_s_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_b_a_d_g_e_/_c_o_o_k_i_e_c_u_t_t_e_r_-_p_y_p_a_c_k_a_g_e_-_s_u_c_c_e_s_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
+_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_]# h-vialib Library functions for use with Via. Usage
+----- This is an internal library, mostly of interest to maintainers of [Via]
+(https://github.com/hypothesis/via) and related components. Some items of
 interest: * [Configuration](https://github.com/hypothesis/h-vialib/blob/main/
 src/h_vialib/configuration.py) - Configuration parameter management ## Setting
 up Your h-vialib Development Environment First you'll need to install: * [Git]
 (https://git-scm.com/). On Ubuntu: `sudo apt install git`, on macOS: `brew
 install git`. * [GNU Make](https://www.gnu.org/software/make/). This is
 probably already installed, run `make --version` to check. * [pyenv](https://
 github.com/pyenv/pyenv). Follow the instructions in pyenv's README to install
```

### Comparing `h-vialib-1.2.2/src/h_vialib.egg-info/SOURCES.txt` & `h_vialib-1.3.0/src/h_vialib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/tests/pyproject.toml` & `h_vialib-1.3.0/tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/tests/unit/h_vialib/_params_test.py` & `h_vialib-1.3.0/tests/unit/h_vialib/_params_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/tests/unit/h_vialib/client_test.py` & `h_vialib-1.3.0/tests/unit/h_vialib/client_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/tests/unit/h_vialib/configuration_test.py` & `h_vialib-1.3.0/tests/unit/h_vialib/configuration_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/tests/unit/h_vialib/secure/encryption_test.py` & `h_vialib-1.3.0/tests/unit/h_vialib/secure/encryption_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-from jose import constants
 
 from h_vialib.secure import Encryption
 
 
 class TestEncryption:
     def test_encrypt_dict_round_trip(self, encryption):
         payload_dict = {"some": "data"}
@@ -14,29 +13,37 @@
 
     def test_encrypt_dict(self, encryption, secret, json, jwe):
         payload_dict = {"some": "data"}
 
         encrypted = encryption.encrypt_dict(payload_dict)
 
         json.dumps.assert_called_with(payload_dict)
-        jwe.encrypt.assert_called_once_with(
-            json.dumps.return_value,
+        jwe.encrypt_compact.assert_called_once_with(
+            {"alg": encryption.JWE_ALGORITHM, "enc": encryption.JWE_ENCRYPTION},
+            json.dumps.return_value.encode.return_value,
             secret.ljust(32),
-            algorithm=constants.ALGORITHMS.DIR,
-            encryption=constants.ALGORITHMS.A128CBC_HS256,
         )
-        assert encrypted == jwe.encrypt.return_value.decode.return_value
+        assert encrypted == jwe.encrypt_compact.return_value
 
-    def test_decrypt_dict(self, encryption, secret, jwe, json):
+    def test_decrypt_dict(self, encryption, secret, json, jwe):
         plain_text_dict = encryption.decrypt_dict("payload")
 
-        jwe.decrypt.assert_called_once_with("payload", secret.ljust(32))
-        json.loads.assert_called_once_with(jwe.decrypt.return_value)
+        jwe.decrypt_compact.assert_called_once_with("payload", secret.ljust(32))
+        json.loads.assert_called_once_with(jwe.decrypt_compact.return_value.plaintext)
         assert plain_text_dict == json.loads.return_value
 
+    def test_decrypt_dict_hardcoded(self, encryption):
+        # Copied from the output of decrypt_dict.
+        # Useful to check backwards compatibility when updating the crypto backend
+        encrypted = "eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..q7UXaHtenyFA5VD3QhrxXA.gkAmUrzmW5UFpuF_tZLmcUzUfS9FuLAiV_xqRJBVJ3Y.U42rUD65NVjH-SoFfeDoOw"
+
+        plain_text_dict = encryption.decrypt_dict(encrypted)
+
+        assert plain_text_dict == {"some": "data"}
+
     @pytest.fixture
     def secret(self):
         return b"VERY SECRET"
 
     @pytest.fixture
     def encryption(self, secret):
         return Encryption(secret)
```

### Comparing `h-vialib-1.2.2/tests/unit/h_vialib/secure/expiry_test.py` & `h_vialib-1.3.0/tests/unit/h_vialib/secure/expiry_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/tests/unit/h_vialib/secure/token_test.py` & `h_vialib-1.3.0/tests/unit/h_vialib/secure/token_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,82 @@
 from datetime import datetime, timedelta
 
 import pytest
 from freezegun import freeze_time
 from h_matchers import Any
-from jose import jwt
-from jose.exceptions import ExpiredSignatureError, JWTError
+from joserfc import jwt
+from joserfc.errors import JoseError
 
 from h_vialib.exceptions import InvalidToken, MissingToken
 from h_vialib.secure.token import SecureToken
 
 
 def decode_token(token_string):
-    return jwt.decode(token_string, "a_very_secret_secret", SecureToken.TOKEN_ALGORITHM)
+    return jwt.decode(token_string, "a_very_secret_secret").claims
+
+
+# This were generated by python-jose but are different than the ones generated by joserfc
+# While the payload is the same the header key order is different:
+#    `typ` & `alg` avs `alg` & `typ`
+# resulting in different tokens.
+# Keeping this around while doing the upgrade for peace of main. We test we can still decode them.
+old_payloads = [
+    (
+        {"a": 2},
+        timedelta(seconds=10),
+        "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhIjoyLCJleHAiOjE2NzE2NjcyMTB9.k5vQWx-k_u_xRDE2wgZhh7DfK75Wt5LnOwDB4tPBA_k",
+    ),
+    (
+        {"a": 2},
+        timedelta(seconds=20),
+        "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhIjoyLCJleHAiOjE2NzE2NjcyMjB9.SZWwElky3JdiR_Xpx1pmQ2k6Kzjnxgm0-KY6AL9Q_Ws",
+    ),
+    (
+        {"b": 5},
+        timedelta(seconds=10),
+        "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJiIjo1LCJleHAiOjE2NzE2NjcyMTB9.Gf1e9jLnn57iGGU4c7nit6zIZ6LWNIQTHiOzk9cLJ9c",
+    ),
+]
 
 
 class TestSecureToken:
     @freeze_time("2022-12-22")
+    @pytest.mark.parametrize("payload,expires,output", old_payloads)
+    def test_old_payloads(self, token, payload, expires, output):
+        exp = int(datetime.now().timestamp() + expires.total_seconds())
+
+        assert token.verify(output) == {**payload, **{"exp": exp}}
+
+    @freeze_time("2022-12-22")
     @pytest.mark.parametrize(
         "payload,expires,output",
         [
             (
                 {"a": 2},
                 timedelta(seconds=10),
-                "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhIjoyLCJleHAiOjE2NzE2NjcyMTB9.k5vQWx-k_u_xRDE2wgZhh7DfK75Wt5LnOwDB4tPBA_k",
+                "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJhIjoyLCJleHAiOjE2NzE2NjcyMTB9.kkQR30rL0dAVL5G6lZEEY-ZwKjulPN-PuhuD5aG29n8",
             ),
             (
                 {"a": 2},
                 timedelta(seconds=20),
-                "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhIjoyLCJleHAiOjE2NzE2NjcyMjB9.SZWwElky3JdiR_Xpx1pmQ2k6Kzjnxgm0-KY6AL9Q_Ws",
+                "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJhIjoyLCJleHAiOjE2NzE2NjcyMjB9.mXogA_p8yXoN7RnkXcio7UOwJa9j8XGKTOdEMf-I3D4",
             ),
             (
                 {"b": 5},
                 timedelta(seconds=10),
-                "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJiIjo1LCJleHAiOjE2NzE2NjcyMTB9.Gf1e9jLnn57iGGU4c7nit6zIZ6LWNIQTHiOzk9cLJ9c",
+                "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJiIjo1LCJleHAiOjE2NzE2NjcyMTB9.J1HgfeeP3e39tX1UlTmYjB4cS6OrarY3EQkuQYHOrhE",
             ),
         ],
     )
     def test_create_output(self, token, payload, expires, output):
         token_string = token.create(payload, expires=datetime.now() + expires)
 
         assert token_string == output
-
-    def test_create_works(self, token):
-        expires = datetime.now() + timedelta(seconds=10)
-
-        token_string = token.create({"a": 2}, expires=expires)
-
-        assert token_string == Any.string()
-        assert decode_token(token_string) == {"a": 2, "exp": Any.int()}
+        # Also assert the opposite operation with the hardcoded tokens
+        assert token.verify(output) == payload
 
     def test_create_works_with_a_max_age(self, token):
         token_string = token.create({"a": 2}, max_age=10)
 
         assert token_string == Any.string()
         assert decode_token(token_string) == {"a": 2, "exp": Any.int()}
 
@@ -62,23 +87,27 @@
     def test_verify_decodes_a_good_token(self, token):
         token_string = token.create({"a": 2}, max_age=10)
 
         decoded = token.verify(token_string)
 
         assert decoded == {"a": 2, "exp": Any.int()}
 
+    @freeze_time("2022-12-22")
+    def test_verify_validates_expiration(self, token):
+        token_string = token.create({"a": 2}, expires=datetime(2021, 1, 1))
+
+        with pytest.raises(InvalidToken):
+            token.verify(token_string)
+
     @pytest.mark.parametrize("token_string", (None, ""))
     def test_verify_catches_there_being_no_value(self, token, token_string):
         with pytest.raises(MissingToken):
             token.verify(token_string)
 
-    @pytest.mark.parametrize(
-        "exception",
-        (JWTError, ExpiredSignatureError),
-    )
+    @pytest.mark.parametrize("exception", [JoseError])
     def test_verify_translates_errors(self, token, jwt, exception):
         jwt.decode.side_effect = exception
         with pytest.raises(InvalidToken):
             token.verify("fake_token")
 
     @pytest.fixture
     def token(self):
```

### Comparing `h-vialib-1.2.2/tests/unit/h_vialib/secure/url_test.py` & `h_vialib-1.3.0/tests/unit/h_vialib/secure/url_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.2/tox.ini` & `h_vialib-1.3.0/tox.ini`

 * *Files identical despite different names*

