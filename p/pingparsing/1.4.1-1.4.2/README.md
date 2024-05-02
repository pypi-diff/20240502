# Comparing `tmp/pingparsing-1.4.1.tar.gz` & `tmp/pingparsing-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pingparsing-1.4.1.tar", last modified: Sat Feb 18 06:46:24 2023, max compression
+gzip compressed data, was "pingparsing-1.4.2.tar", last modified: Thu May  2 09:34:19 2024, max compression
```

## Comparing `pingparsing-1.4.1.tar` & `pingparsing-1.4.2.tar`

### file list

```diff
@@ -1,54 +1,93 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-18 06:46:24.258561 pingparsing-1.4.1/
--rw-r--r--   0 toor      (1000) toor      (1000)     1084 2023-02-18 06:44:41.000000 pingparsing-1.4.1/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      242 2023-02-18 06:44:41.000000 pingparsing-1.4.1/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)    22359 2023-02-18 06:46:24.258561 pingparsing-1.4.1/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)    20416 2023-02-18 06:44:41.000000 pingparsing-1.4.1/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-18 06:46:24.238561 pingparsing-1.4.1/docs/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-18 06:46:24.238561 pingparsing-1.4.1/docs/pages/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-18 06:46:24.248561 pingparsing-1.4.1/docs/pages/introduction/
--rw-r--r--   0 toor      (1000) toor      (1000)       82 2023-02-18 06:44:41.000000 pingparsing-1.4.1/docs/pages/introduction/summary.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-18 06:46:24.248561 pingparsing-1.4.1/examples/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-02-18 06:44:41.000000 pingparsing-1.4.1/examples/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1202 2023-02-18 06:44:41.000000 pingparsing-1.4.1/examples/examplecommon.py
--rwxr-xr-x   0 toor      (1000) toor      (1000)     1268 2023-02-18 06:44:41.000000 pingparsing-1.4.1/examples/parse_sample.py
--rwxr-xr-x   0 toor      (1000) toor      (1000)      498 2023-02-18 06:44:41.000000 pingparsing-1.4.1/examples/ping_sample.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-18 06:46:24.248561 pingparsing-1.4.1/pingparsing/
--rw-r--r--   0 toor      (1000) toor      (1000)      364 2023-02-18 06:44:41.000000 pingparsing-1.4.1/pingparsing/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    11919 2023-02-18 06:44:41.000000 pingparsing-1.4.1/pingparsing/__main__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-02-18 06:44:41.000000 pingparsing-1.4.1/pingparsing/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7011 2023-02-18 06:44:41.000000 pingparsing-1.4.1/pingparsing/_cmd_maker.py
--rw-r--r--   0 toor      (1000) toor      (1000)      274 2023-02-18 06:44:41.000000 pingparsing-1.4.1/pingparsing/_common.py
--rw-r--r--   0 toor      (1000) toor      (1000)      242 2023-02-18 06:44:41.000000 pingparsing-1.4.1/pingparsing/_interface.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1691 2023-02-18 06:44:41.000000 pingparsing-1.4.1/pingparsing/_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)    17965 2023-02-18 06:44:41.000000 pingparsing-1.4.1/pingparsing/_parser.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2526 2023-02-18 06:44:41.000000 pingparsing-1.4.1/pingparsing/_pingparsing.py
--rw-r--r--   0 toor      (1000) toor      (1000)    10840 2023-02-18 06:44:41.000000 pingparsing-1.4.1/pingparsing/_pingtransmitter.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6899 2023-02-18 06:44:41.000000 pingparsing-1.4.1/pingparsing/_stats.py
--rw-r--r--   0 toor      (1000) toor      (1000)      256 2023-02-18 06:44:41.000000 pingparsing-1.4.1/pingparsing/_typing.py
--rw-r--r--   0 toor      (1000) toor      (1000)      580 2023-02-18 06:44:41.000000 pingparsing-1.4.1/pingparsing/error.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-02-18 06:44:41.000000 pingparsing-1.4.1/pingparsing/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-18 06:46:24.248561 pingparsing-1.4.1/pingparsing.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)    22359 2023-02-18 06:46:24.000000 pingparsing-1.4.1/pingparsing.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     1032 2023-02-18 06:46:24.000000 pingparsing-1.4.1/pingparsing.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-02-18 06:46:24.000000 pingparsing-1.4.1/pingparsing.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       58 2023-02-18 06:46:24.000000 pingparsing-1.4.1/pingparsing.egg-info/entry_points.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      200 2023-02-18 06:46:24.000000 pingparsing-1.4.1/pingparsing.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       21 2023-02-18 06:46:24.000000 pingparsing-1.4.1/pingparsing.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1271 2023-02-18 06:44:41.000000 pingparsing-1.4.1/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-18 06:46:24.248561 pingparsing-1.4.1/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       43 2023-02-18 06:44:41.000000 pingparsing-1.4.1/requirements/docs_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       93 2023-02-18 06:44:41.000000 pingparsing-1.4.1/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       58 2023-02-18 06:44:41.000000 pingparsing-1.4.1/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-02-18 06:46:24.258561 pingparsing-1.4.1/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     3426 2023-02-18 06:44:41.000000 pingparsing-1.4.1/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-18 06:46:24.258561 pingparsing-1.4.1/test/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-02-18 06:44:41.000000 pingparsing-1.4.1/test/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      321 2023-02-18 06:44:41.000000 pingparsing-1.4.1/test/common.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9677 2023-02-18 06:44:41.000000 pingparsing-1.4.1/test/data.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9188 2023-02-18 06:44:41.000000 pingparsing-1.4.1/test/test_cli.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5729 2023-02-18 06:44:41.000000 pingparsing-1.4.1/test/test_cmd_maker.py
--rw-r--r--   0 toor      (1000) toor      (1000)      537 2023-02-18 06:44:41.000000 pingparsing-1.4.1/test/test_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)    25891 2023-02-18 06:44:41.000000 pingparsing-1.4.1/test/test_pingparsing.py
--rw-r--r--   0 toor      (1000) toor      (1000)      599 2023-02-18 06:44:41.000000 pingparsing-1.4.1/test/test_pingresult.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5441 2023-02-18 06:44:41.000000 pingparsing-1.4.1/test/test_pingtransmitter.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1436 2023-02-18 06:44:41.000000 pingparsing-1.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:34:19.329697 pingparsing-1.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:34:19.317698 pingparsing-1.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-02 09:33:43.000000 pingparsing-1.4.2/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-02 09:33:43.000000 pingparsing-1.4.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:34:19.317698 pingparsing-1.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-02 09:33:43.000000 pingparsing-1.4.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-02 09:33:43.000000 pingparsing-1.4.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-02 09:33:43.000000 pingparsing-1.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-02 09:33:43.000000 pingparsing-1.4.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-05-02 09:33:43.000000 pingparsing-1.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-02 09:33:43.000000 pingparsing-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-02 09:33:43.000000 pingparsing-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-02 09:33:43.000000 pingparsing-1.4.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    23759 2024-05-02 09:34:19.329697 pingparsing-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21123 2024-05-02 09:33:43.000000 pingparsing-1.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:34:19.317698 pingparsing-1.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10219 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/make_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:34:19.317698 pingparsing-1.4.2/docs/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/changelog_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:34:19.321698 pingparsing-1.4.2/docs/pages/introduction/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/introduction/badges.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/introduction/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/introduction/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/introduction/premise.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/introduction/summary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/introduction/supported_environment.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/links.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:34:19.321698 pingparsing-1.4.2/docs/pages/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/reference/error.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/reference/parser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/reference/transmitter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/sponsors.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:34:19.321698 pingparsing-1.4.2/docs/pages/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/usage/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/usage/cli_help.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/usage/cli_usage.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/usage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/pages/usage/library.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-05-02 09:33:43.000000 pingparsing-1.4.2/docs/update_command_help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:34:19.321698 pingparsing-1.4.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:33:43.000000 pingparsing-1.4.2/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-02 09:33:43.000000 pingparsing-1.4.2/examples/examplecommon.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1268 2024-05-02 09:33:43.000000 pingparsing-1.4.2/examples/parse_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 09:33:43.000000 pingparsing-1.4.2/examples/ping.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      498 2024-05-02 09:33:43.000000 pingparsing-1.4.2/examples/ping_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-02 09:33:43.000000 pingparsing-1.4.2/examples/ping_win7.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:34:19.325698 pingparsing-1.4.2/pingparsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-02 09:33:43.000000 pingparsing-1.4.2/pingparsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11987 2024-05-02 09:33:43.000000 pingparsing-1.4.2/pingparsing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 09:33:43.000000 pingparsing-1.4.2/pingparsing/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-02 09:33:43.000000 pingparsing-1.4.2/pingparsing/_cmd_maker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 09:33:43.000000 pingparsing-1.4.2/pingparsing/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-02 09:33:43.000000 pingparsing-1.4.2/pingparsing/_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-02 09:33:43.000000 pingparsing-1.4.2/pingparsing/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18013 2024-05-02 09:33:43.000000 pingparsing-1.4.2/pingparsing/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-02 09:33:43.000000 pingparsing-1.4.2/pingparsing/_pingparsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-05-02 09:33:43.000000 pingparsing-1.4.2/pingparsing/_pingtransmitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-05-02 09:33:43.000000 pingparsing-1.4.2/pingparsing/_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-02 09:33:43.000000 pingparsing-1.4.2/pingparsing/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-02 09:33:43.000000 pingparsing-1.4.2/pingparsing/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:33:43.000000 pingparsing-1.4.2/pingparsing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:34:19.329697 pingparsing-1.4.2/pingparsing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23759 2024-05-02 09:34:19.000000 pingparsing-1.4.2/pingparsing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-02 09:34:19.000000 pingparsing-1.4.2/pingparsing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 09:34:19.000000 pingparsing-1.4.2/pingparsing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-02 09:34:19.000000 pingparsing-1.4.2/pingparsing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-02 09:34:19.000000 pingparsing-1.4.2/pingparsing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 09:34:19.000000 pingparsing-1.4.2/pingparsing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-02 09:33:43.000000 pingparsing-1.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:34:19.325698 pingparsing-1.4.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 09:33:43.000000 pingparsing-1.4.2/requirements/docs_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 09:33:43.000000 pingparsing-1.4.2/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-02 09:33:43.000000 pingparsing-1.4.2/requirements/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 09:34:19.329697 pingparsing-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-02 09:33:43.000000 pingparsing-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:34:19.329697 pingparsing-1.4.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:33:43.000000 pingparsing-1.4.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-02 09:33:43.000000 pingparsing-1.4.2/test/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-05-02 09:33:43.000000 pingparsing-1.4.2/test/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-05-02 09:33:43.000000 pingparsing-1.4.2/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-02 09:33:43.000000 pingparsing-1.4.2/test/test_cmd_maker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-02 09:33:43.000000 pingparsing-1.4.2/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26602 2024-05-02 09:33:43.000000 pingparsing-1.4.2/test/test_pingparsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-02 09:33:43.000000 pingparsing-1.4.2/test/test_pingresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-05-02 09:33:43.000000 pingparsing-1.4.2/test/test_pingtransmitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-02 09:33:43.000000 pingparsing-1.4.2/tox.ini
```

### Comparing `pingparsing-1.4.1/LICENSE` & `pingparsing-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pingparsing-1.4.1/PKG-INFO` & `pingparsing-1.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pingparsing
-Version: 1.4.1
-Summary: pingparsing is a CLI-tool/Python-library parser and transmitter for ping command.
+Version: 1.4.2
+Summary: pingparsing is a CLI-tool/Python-library parser and transmitter for the ping command.
 Home-page: https://github.com/thombashi/pingparsing
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
+Project-URL: Changelog, https://github.com/thombashi/pingparsing/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://pingparsing.rtfd.io/
 Project-URL: Source, https://github.com/thombashi/pingparsing
 Project-URL: Tracker, https://github.com/thombashi/pingparsing/issues
 Keywords: cli,library,network,ping,parser,transmitter
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -17,60 +18,76 @@
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: Text Processing
-Requires-Python: >=3.6
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: humanreadable<1,>=0.3
+Requires-Dist: pyparsing<4,>=2.0.3
+Requires-Dist: subprocrunner<3,>=1.2.2
+Requires-Dist: typepy[datetime]<2,>=1.3.2
+Provides-Extra: docs
+Requires-Dist: sphinx_rtd_theme>=1.2.2; extra == "docs"
+Requires-Dist: Sphinx>=2.4; extra == "docs"
+Requires-Dist: subprocrunner; extra == "docs"
 Provides-Extra: test
+Requires-Dist: pytest>=6.0.1; extra == "test"
+Requires-Dist: pytest-discord>=0.1.6; extra == "test"
+Requires-Dist: pytest-md-report>=0.5; extra == "test"
 Provides-Extra: cli
-License-File: LICENSE
+Requires-Dist: loguru<1,>=0.4.1; extra == "cli"
+Requires-Dist: Pygments<3,>=2.1; extra == "cli"
 
 .. contents:: **pingparsing**
    :backlinks: top
    :depth: 2
 
 Summary
 =========
-`pingparsing <https://github.com/thombashi/pingparsing>`__ is a CLI-tool/Python-library parser and transmitter for ping command.
+`pingparsing <https://github.com/thombashi/pingparsing>`__ is a CLI-tool/Python-library parser and transmitter for the ping command.
 
-.. image:: https://badge.fury.io/py/pingparsing.svg
+|PyPI pkg ver| |Supported Python impl| |Supported Python ver| |CI status| |CodeQL|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/pingparsing.svg
     :target: https://badge.fury.io/py/pingparsing
     :alt: PyPI package version
 
-.. image:: https://img.shields.io/pypi/pyversions/pingparsing.svg
+.. |Supported Python impl| image:: https://img.shields.io/pypi/implementation/pingparsing.svg
     :target: https://pypi.org/project/pingparsing
-    :alt: Supported Python versions
+    :alt: Supported Python implementations
 
-.. image:: https://img.shields.io/pypi/implementation/pingparsing.svg
+.. |Supported Python ver| image:: https://img.shields.io/pypi/pyversions/pingparsing.svg
     :target: https://pypi.org/project/pingparsing
-    :alt: Supported Python implementations
+    :alt: Supported Python versions
 
-.. image:: https://github.com/thombashi/pingparsing/workflows/Tests/badge.svg
-    :target: https://github.com/thombashi/pingparsing/actions?query=workflow%3ATests
-    :alt: Linux/macOS/Windows CI status
+.. |CI status| image:: https://github.com/thombashi/pingparsing/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/pingparsing/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
 
-.. image:: https://github.com/thombashi/pingparsing/actions/workflows/codeql-analysis.yml/badge.svg
-    :target: https://github.com/thombashi/pingparsing/actions/workflows/codeql-analysis.yml
+.. |CodeQL| image:: https://github.com/thombashi/pingparsing/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/pingparsing/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
 CLI Usage
 ====================
 A CLI command (``pingparsing`` command) is included in the package. The command could do the following:
 
 - Execute ``ping`` and parse the result
@@ -525,15 +542,15 @@
 ::
 
     pip install pingparsing
 
 
 Dependencies
 ============
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pingparsing/network/dependencies>`__
 
 Optional Dependencies
 ------------------------------------
 - pingparsing[cli] extras
     - `loguru <https://github.com/Delgan/loguru>`__
         - Used for logging if the package installed
@@ -559,14 +576,16 @@
 +==============+===================================+
 | Ubuntu 16.04 | ``iputils-ping 20121221-5ubuntu2``|
 +--------------+-----------------------------------+
 | Ubuntu 18.04 | ``iputils-ping 20161105-1ubuntu2``|
 +--------------+-----------------------------------+
 | Ubuntu 20.04 | ``iputils-ping 20190709-3``       |
 +--------------+-----------------------------------+
+| Ubuntu 22.04 | ``iputils-ping 20211215-1``       |
++--------------+-----------------------------------+
 | Debian 8.6   | ``iputils-ping 20121221-5+b2``    |
 +--------------+-----------------------------------+
 | Fedora 25    | ``iputils-20161105-1.fc25.x86_64``|
 +--------------+-----------------------------------+
 | Windows 10   | ``-``                             |
 +--------------+-----------------------------------+
 | macOS 10.13  | ``-``                             |
@@ -580,19 +599,27 @@
 
 Documentation
 ===============
 https://pingparsing.rtfd.io/
 
 Sponsors
 ====================================
-.. image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
+|chasbecker| |shiguredo| |b4tman| |Arturi0| |github|
+
+.. |chasbecker| image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
    :target: https://github.com/chasbecker
-   :alt: Charles Becker (chasbecker)
-.. image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
-   :target: https://github.com/Arturi0
-   :alt: onetime: Arturi0
-.. image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
+   :alt: ex-sponsor: Charles Becker (chasbecker)
+.. |shiguredo| image:: https://avatars.githubusercontent.com/u/2549434?s=48&v=4
+   :target: https://github.com/shiguredo
+   :alt: ex-sponsor: 時雨堂 (shiguredo)
+.. |b4tman| image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
    :target: https://github.com/b4tman
    :alt: onetime: Dmitry Belyaev (b4tman)
+.. |Arturi0| image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
+   :target: https://github.com/Arturi0
+   :alt: onetime: Arturi0
+.. |github| image:: https://avatars.githubusercontent.com/u/9919?s=48&v=4
+   :target: https://github.com/github
+   :alt: onetime: GitHub (github)
 
 `Become a sponsor <https://github.com/sponsors/thombashi>`__
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pingparsing-1.4.1/README.rst` & `pingparsing-1.4.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 .. contents:: **pingparsing**
    :backlinks: top
    :depth: 2
 
 Summary
 =========
-`pingparsing <https://github.com/thombashi/pingparsing>`__ is a CLI-tool/Python-library parser and transmitter for ping command.
+`pingparsing <https://github.com/thombashi/pingparsing>`__ is a CLI-tool/Python-library parser and transmitter for the ping command.
 
-.. image:: https://badge.fury.io/py/pingparsing.svg
+|PyPI pkg ver| |Supported Python impl| |Supported Python ver| |CI status| |CodeQL|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/pingparsing.svg
     :target: https://badge.fury.io/py/pingparsing
     :alt: PyPI package version
 
-.. image:: https://img.shields.io/pypi/pyversions/pingparsing.svg
+.. |Supported Python impl| image:: https://img.shields.io/pypi/implementation/pingparsing.svg
     :target: https://pypi.org/project/pingparsing
-    :alt: Supported Python versions
+    :alt: Supported Python implementations
 
-.. image:: https://img.shields.io/pypi/implementation/pingparsing.svg
+.. |Supported Python ver| image:: https://img.shields.io/pypi/pyversions/pingparsing.svg
     :target: https://pypi.org/project/pingparsing
-    :alt: Supported Python implementations
+    :alt: Supported Python versions
 
-.. image:: https://github.com/thombashi/pingparsing/workflows/Tests/badge.svg
-    :target: https://github.com/thombashi/pingparsing/actions?query=workflow%3ATests
-    :alt: Linux/macOS/Windows CI status
+.. |CI status| image:: https://github.com/thombashi/pingparsing/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/pingparsing/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
 
-.. image:: https://github.com/thombashi/pingparsing/actions/workflows/codeql-analysis.yml/badge.svg
-    :target: https://github.com/thombashi/pingparsing/actions/workflows/codeql-analysis.yml
+.. |CodeQL| image:: https://github.com/thombashi/pingparsing/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/pingparsing/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
 CLI Usage
 ====================
 A CLI command (``pingparsing`` command) is included in the package. The command could do the following:
 
 - Execute ``ping`` and parse the result
@@ -482,15 +484,15 @@
 ::
 
     pip install pingparsing
 
 
 Dependencies
 ============
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pingparsing/network/dependencies>`__
 
 Optional Dependencies
 ------------------------------------
 - pingparsing[cli] extras
     - `loguru <https://github.com/Delgan/loguru>`__
         - Used for logging if the package installed
@@ -516,14 +518,16 @@
 +==============+===================================+
 | Ubuntu 16.04 | ``iputils-ping 20121221-5ubuntu2``|
 +--------------+-----------------------------------+
 | Ubuntu 18.04 | ``iputils-ping 20161105-1ubuntu2``|
 +--------------+-----------------------------------+
 | Ubuntu 20.04 | ``iputils-ping 20190709-3``       |
 +--------------+-----------------------------------+
+| Ubuntu 22.04 | ``iputils-ping 20211215-1``       |
++--------------+-----------------------------------+
 | Debian 8.6   | ``iputils-ping 20121221-5+b2``    |
 +--------------+-----------------------------------+
 | Fedora 25    | ``iputils-20161105-1.fc25.x86_64``|
 +--------------+-----------------------------------+
 | Windows 10   | ``-``                             |
 +--------------+-----------------------------------+
 | macOS 10.13  | ``-``                             |
@@ -537,19 +541,27 @@
 
 Documentation
 ===============
 https://pingparsing.rtfd.io/
 
 Sponsors
 ====================================
-.. image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
+|chasbecker| |shiguredo| |b4tman| |Arturi0| |github|
+
+.. |chasbecker| image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
    :target: https://github.com/chasbecker
-   :alt: Charles Becker (chasbecker)
-.. image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
-   :target: https://github.com/Arturi0
-   :alt: onetime: Arturi0
-.. image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
+   :alt: ex-sponsor: Charles Becker (chasbecker)
+.. |shiguredo| image:: https://avatars.githubusercontent.com/u/2549434?s=48&v=4
+   :target: https://github.com/shiguredo
+   :alt: ex-sponsor: 時雨堂 (shiguredo)
+.. |b4tman| image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
    :target: https://github.com/b4tman
    :alt: onetime: Dmitry Belyaev (b4tman)
+.. |Arturi0| image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
+   :target: https://github.com/Arturi0
+   :alt: onetime: Arturi0
+.. |github| image:: https://avatars.githubusercontent.com/u/9919?s=48&v=4
+   :target: https://github.com/github
+   :alt: onetime: GitHub (github)
 
 `Become a sponsor <https://github.com/sponsors/thombashi>`__
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pingparsing-1.4.1/examples/examplecommon.py` & `pingparsing-1.4.2/examples/examplecommon.py`

 * *Files identical despite different names*

### Comparing `pingparsing-1.4.1/examples/parse_sample.py` & `pingparsing-1.4.2/examples/parse_sample.py`

 * *Files identical despite different names*

### Comparing `pingparsing-1.4.1/pingparsing/__main__.py` & `pingparsing-1.4.2/pingparsing/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,17 +81,15 @@
         "--timestamp",
         choices=TimestampFormat.LIST,
         default=TimestampFormat.NONE,
         help="""[Only for LINUX]
         {}: no timestamps.
         {}: add timestamps with UNIX epoch time format.
         {}: add timestamps with ISO time format.
-        """.format(
-            TimestampFormat.NONE, TimestampFormat.EPOCH, TimestampFormat.DATETIME
-        ),
+        """.format(TimestampFormat.NONE, TimestampFormat.EPOCH, TimestampFormat.DATETIME),
     )
     group.add_argument(
         "-c",
         "--count",
         type=int,
         help="""Stop after sending the count.
         see also ping(8) [-c count] option description.
@@ -109,39 +107,35 @@
         help="Specifies the Time to Live.",
     )
     group.add_argument(
         "-w",
         "--deadline",
         type=str,
         help="""Timeout before ping exits.
-        valid time units are: {units}. if no unit string found, considered seconds as
+        valid time units are: {units}. if no unit string is found, consider seconds as
         the time unit.
 
         see also ping(8) [-w deadline] option description.
-        note: meaning of the 'deadline' may differ system from to system.
-        """.format(
-            units=_get_unit_help_msg()
-        ),
+        note: The meaning of the 'deadline' may differ system from to system.
+        """.format(units=_get_unit_help_msg()),
     )
     group.add_argument(
         "--timeout",
         type=str,
         help="""Time to wait for a response per packet.
         Valid time units are: {units}.
         If no unit string is found, consider milliseconds as the time unit.
         Attempt to send packets with milliseconds granularity in default.
         If the system does not support timeout in milliseconds, round up as seconds.
         Use system default if not specified.
         This option will be ignored if the system does not support timeout itself.
 
         See also ping(8) [-W timeout] option description.
-        note: meaning of the 'timeout' may differ from system to system.
-        """.format(
-            units=_get_unit_help_msg()
-        ),
+        note: The meaning of the 'timeout' may differ from system to system.
+        """.format(units=_get_unit_help_msg()),
     )
     group.add_argument("-I", "--interface", dest="interface", help="network interface")
     group.add_argument("--addopts", metavar="OPTIONS", help="extra command line options")
 
     group = parser.add_argument_group("Output Options")  # type: ignore
     group.add_argument(
         "--indent",
@@ -247,16 +241,16 @@
     else:
         transmitter = PingTransmitter()
         transmitter.destination = dest_or_file
         transmitter.interface = interface
         transmitter.count = count
         transmitter.packet_size = packet_size
         transmitter.ttl = ttl
-        transmitter.deadline = deadline
-        transmitter.timeout = timeout
+        transmitter.deadline = deadline  # type: ignore
+        transmitter.timeout = timeout  # type: ignore
         transmitter.is_quiet = not is_parse_icmp_reply
         transmitter.timestamp = timestamp != TimestampFormat.NONE
         transmitter.ping_option = addopts
 
         try:
             result = transmitter.ping()
         except CommandError as e:
@@ -275,21 +269,23 @@
 
     stats = ping_parser.parse(ping_result_text)
     output = stats.as_dict(include_icmp_replies=is_parse_icmp_reply)
 
     return (dest_or_file, output)
 
 
-def get_ping_param(options) -> Tuple:
-    count = options.count
-    deadline = options.deadline
-    timeout = options.timeout
+def get_ping_param(ns: argparse.Namespace) -> Tuple[int, TimeArg, TimeArg]:
+    count: int
+    deadline: TimeArg = ns.deadline
+    timeout: TimeArg = ns.timeout
 
-    if not options.count and not options.deadline:
+    if not ns.count and not ns.deadline:
         count = DEFAULT_COUNT
+    else:
+        count = ns.count
 
     return (count, deadline, timeout)
 
 
 def print_result(text: str, colorize: bool) -> None:
     if not sys.stdout.isatty() or not colorize:
         # avoid to colorized when piped or redirected
@@ -299,15 +295,17 @@
     try:
         from pygments import highlight
         from pygments.formatters import TerminalTrueColorFormatter
         from pygments.lexers import JsonLexer
 
         print(
             highlight(
-                code=text, lexer=JsonLexer(), formatter=TerminalTrueColorFormatter(style="monokai")
+                code=text,
+                lexer=JsonLexer(),
+                formatter=TerminalTrueColorFormatter(style="monokai"),
             ).strip()
         )
     except ImportError:
         print(text)
 
 
 def _serialize_epoch(obj):
```

### Comparing `pingparsing-1.4.1/pingparsing/_cmd_maker.py` & `pingparsing-1.4.2/pingparsing/_cmd_maker.py`

 * *Files identical despite different names*

### Comparing `pingparsing-1.4.1/pingparsing/_logger.py` & `pingparsing-1.4.2/pingparsing/_logger.py`

 * *Files identical despite different names*

### Comparing `pingparsing-1.4.1/pingparsing/_parser.py` & `pingparsing-1.4.2/pingparsing/_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,35 +39,39 @@
     _ICMP_SEQ_PATTERN = rf"\s*icmp_seq=(?P<{IcmpReplyKey.SEQUENCE_NO}>\d+)"
     _TTL_PATTERN = rf"\s*ttl=(?P<{IcmpReplyKey.TTL}>\d+)"
     _TIME_PATTERN = rf"\s*time[=<](?P<{IcmpReplyKey.TIME}>[0-9\.]+)"
 
     def __init__(self, timezone: Optional[tzinfo] = None) -> None:
         self.__timezone = timezone
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def _parser_name(self) -> str:  # pragma: no cover
         pass
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def _icmp_reply_pattern(self) -> str:  # pragma: no cover
         pass
 
     @property
     def _icmp_no_ans_pattern(self) -> str:
         return "(?!x)x"  # never matching anything
 
     @property
     def _duplicate_packet_pattern(self) -> str:
         return r".+ \(DUP!\)$"
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def _stats_headline_pattern(self) -> str:  # pragma: no cover
         pass
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def _is_support_packet_duplicate(self) -> bool:  # pragma: no cover
         pass
 
     def _parse_icmp_reply(self, ping_lines: Sequence[str]) -> IcmpReplies:
         icmp_reply_regexp = re.compile(self._icmp_reply_pattern, re.IGNORECASE)
         icmp_no_ans_regexp = re.compile(self._icmp_no_ans_pattern, re.IGNORECASE)
         duplicate_packet_regexp = re.compile(self._duplicate_packet_pattern)
```

### Comparing `pingparsing-1.4.1/pingparsing/_pingparsing.py` & `pingparsing-1.4.2/pingparsing/_pingparsing.py`

 * *Files identical despite different names*

### Comparing `pingparsing-1.4.1/pingparsing/_pingtransmitter.py` & `pingparsing-1.4.2/pingparsing/_pingtransmitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     Transmitter class to send ICMP packets by using the OS built-in ``ping``
     command.
 
     .. py:attribute:: count
         :type: Optional[int]
         :value: None
 
-        Number of sending ICMP packets. This attribute ignored if the value is |None|.
+        Number of sending ICMP packets. This attribute will be ignored if the value is |None|.
 
     .. py:attribute:: packet_size
         :type: Optional[int]
         :value: None
 
         Specifies the number of data bytes to be sent.
 
@@ -78,29 +78,29 @@
         Interface name or zone-id. The attribute required when
         :py:attr:`~.destination` is IPv6 link-local scope address.
 
     .. py:attribute:: timestamp
         :type: bool
         :value: False
 
-        [Only for Linux environment] If |True|, add timestamp for each ping result.
+        [Only for Linux environment] If |True|, add a timestamp for each ping result.
         Defaults to ``False``.
 
     .. py:attribute:: auto_codepage
         :type: bool
         :value: True
 
-        [Only for Windows environment] Automatically change code page if
-        ``True``. Defaults to ``True``.
+        [Only for Windows environment] Automatically change the code page if ``True``.
+        Defaults to ``True``.
     """
 
     @property
     def destination(self) -> str:
         """
-        Hostname or IP-address (IPv4/IPv6) to sending ICMP packets.
+        Hostname or IP address (IPv4/IPv6) to send ICMP packets.
         """
 
         return self.__destination
 
     @destination.setter
     def destination(self, value: str) -> None:
         if not String(value, strict_level=StrictLevel.MAX).is_type():
@@ -121,15 +121,16 @@
         self.destination = value
 
     @property
     def timeout(self) -> Optional[hr.Time]:
         """
         Time to wait for a response per packet.
         You can specify either a number or a string (e.g. ``"1sec"``).
-        If only a number is specified and a unit not found, the unit will be considered as seconds.
+        If only a number is specified and a unit is not found,
+        the unit will be considered as seconds.
 
             +------------+----------------------------------------------------------+
             |    Unit    |                Available specifiers (str)                |
             +============+==========================================================+
             |days        |``d``/``day``/``days``                                    |
             +------------+----------------------------------------------------------+
             |hours       |``h``/``hour``/``hours``                                  |
@@ -156,29 +157,30 @@
     @timeout.setter
     def timeout(self, value: TimeArg) -> None:
         if value is None:
             self.__timeout: Optional[hr.Time] = value
             return
 
         if isinstance(value, hr.Time):
-            timeout = cast(hr.Time, value)
+            new_timeout = cast(hr.Time, value)
         else:
-            timeout = hr.Time(str(value), default_unit=hr.Time.Unit.MILLISECOND)
+            new_timeout = hr.Time(str(value), default_unit=hr.Time.Unit.MILLISECOND)
 
-        if timeout.milliseconds <= 0:
+        if new_timeout.milliseconds <= 0:
             raise ValueError("timeout must be greater than zero")
 
-        self.__timeout = cast(hr.Time, timeout)
+        self.__timeout = cast(hr.Time, new_timeout)
 
     @property
     def deadline(self) -> Optional[hr.Time]:
         """
         Timeout before ping exits.
         You can specify either a number or a string (e.g. ``"1sec"``).
-        If only a number is specified and a unit not found, the unit will be considered as seconds.
+        If only a number is specified and a unit is not found,
+        the unit will be considered as seconds.
 
             +------------+----------------------------------------------------------+
             |    Unit    |                Available specifiers (str)                |
             +============+==========================================================+
             |days        |``d``/``day``/``days``                                    |
             +------------+----------------------------------------------------------+
             |hours       |``h``/``hour``/``hours``                                  |
@@ -205,44 +207,44 @@
     @deadline.setter
     def deadline(self, value: TimeArg) -> None:
         if value is None:
             self.__deadline = value
             return
 
         if isinstance(value, hr.Time):
-            deadline = cast(hr.Time, value)
+            new_deadline = cast(hr.Time, value)
         else:
-            deadline = hr.Time(str(value), default_unit=hr.Time.Unit.SECOND)
+            new_deadline = hr.Time(str(value), default_unit=hr.Time.Unit.SECOND)
 
-        if deadline.milliseconds <= 0:
+        if new_deadline.milliseconds <= 0:
             raise ValueError("deadline must be greater than zero")
 
-        self.__deadline = deadline
+        self.__deadline = new_deadline
 
     def __init__(self) -> None:
         self.__destination = ""
         self.count: Optional[int] = None
         self.packet_size: Optional[int] = None
         self.ttl: Optional[int] = None
         self.ping_option: PingAddOpts = []
         self.is_quiet = False
         self.interface: Optional[str] = None
         self.auto_codepage = True
 
-        self.timeout = None
-        self.deadline = None
+        self.timeout: TimeArg = None
+        self.deadline: TimeArg = None
         self.timestamp = False
 
     def ping(self) -> PingResult:
         """
         Sending ICMP packets.
 
         :return: ``ping`` command execution result.
         :rtype: :py:class:`.PingResult`
-        :raises ValueError: If parameters not valid.
+        :raises ValueError: If parameters are not valid.
         """
 
         self.__validate_ping_param()
 
         ping_runner = subprocrunner.SubprocessRunner(self.__make_ping_command())
         ping_runner.run()
```

### Comparing `pingparsing-1.4.1/pingparsing/_stats.py` & `pingparsing-1.4.2/pingparsing/_stats.py`

 * *Files identical despite different names*

### Comparing `pingparsing-1.4.1/pingparsing/error.py` & `pingparsing-1.4.2/pingparsing/error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import enum
-from typing import Union
+from typing import Optional
 
 
 @enum.unique
 class ParseErrorReason(enum.Enum):
     HEADER_NOT_FOUND = "ping statistics not found"
     EMPTY_STATISTICS = "ping statistics is empty"
 
 
 class ParseError(Exception):
     """
     Exception raised when failed to parse ping results.
     """
 
     @property
-    def reason(self) -> Union[str]:
+    def reason(self) -> Optional[str]:
         return self.__reason
 
     def __init__(self, *args, **kwargs):
         self.__reason = kwargs.pop("reason", None)
 
         super().__init__(*args, **kwargs)
```

### Comparing `pingparsing-1.4.1/pingparsing.egg-info/PKG-INFO` & `pingparsing-1.4.2/pingparsing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pingparsing
-Version: 1.4.1
-Summary: pingparsing is a CLI-tool/Python-library parser and transmitter for ping command.
+Version: 1.4.2
+Summary: pingparsing is a CLI-tool/Python-library parser and transmitter for the ping command.
 Home-page: https://github.com/thombashi/pingparsing
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
+Project-URL: Changelog, https://github.com/thombashi/pingparsing/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://pingparsing.rtfd.io/
 Project-URL: Source, https://github.com/thombashi/pingparsing
 Project-URL: Tracker, https://github.com/thombashi/pingparsing/issues
 Keywords: cli,library,network,ping,parser,transmitter
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -17,60 +18,76 @@
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: Text Processing
-Requires-Python: >=3.6
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: humanreadable<1,>=0.3
+Requires-Dist: pyparsing<4,>=2.0.3
+Requires-Dist: subprocrunner<3,>=1.2.2
+Requires-Dist: typepy[datetime]<2,>=1.3.2
+Provides-Extra: docs
+Requires-Dist: sphinx_rtd_theme>=1.2.2; extra == "docs"
+Requires-Dist: Sphinx>=2.4; extra == "docs"
+Requires-Dist: subprocrunner; extra == "docs"
 Provides-Extra: test
+Requires-Dist: pytest>=6.0.1; extra == "test"
+Requires-Dist: pytest-discord>=0.1.6; extra == "test"
+Requires-Dist: pytest-md-report>=0.5; extra == "test"
 Provides-Extra: cli
-License-File: LICENSE
+Requires-Dist: loguru<1,>=0.4.1; extra == "cli"
+Requires-Dist: Pygments<3,>=2.1; extra == "cli"
 
 .. contents:: **pingparsing**
    :backlinks: top
    :depth: 2
 
 Summary
 =========
-`pingparsing <https://github.com/thombashi/pingparsing>`__ is a CLI-tool/Python-library parser and transmitter for ping command.
+`pingparsing <https://github.com/thombashi/pingparsing>`__ is a CLI-tool/Python-library parser and transmitter for the ping command.
 
-.. image:: https://badge.fury.io/py/pingparsing.svg
+|PyPI pkg ver| |Supported Python impl| |Supported Python ver| |CI status| |CodeQL|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/pingparsing.svg
     :target: https://badge.fury.io/py/pingparsing
     :alt: PyPI package version
 
-.. image:: https://img.shields.io/pypi/pyversions/pingparsing.svg
+.. |Supported Python impl| image:: https://img.shields.io/pypi/implementation/pingparsing.svg
     :target: https://pypi.org/project/pingparsing
-    :alt: Supported Python versions
+    :alt: Supported Python implementations
 
-.. image:: https://img.shields.io/pypi/implementation/pingparsing.svg
+.. |Supported Python ver| image:: https://img.shields.io/pypi/pyversions/pingparsing.svg
     :target: https://pypi.org/project/pingparsing
-    :alt: Supported Python implementations
+    :alt: Supported Python versions
 
-.. image:: https://github.com/thombashi/pingparsing/workflows/Tests/badge.svg
-    :target: https://github.com/thombashi/pingparsing/actions?query=workflow%3ATests
-    :alt: Linux/macOS/Windows CI status
+.. |CI status| image:: https://github.com/thombashi/pingparsing/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/pingparsing/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
 
-.. image:: https://github.com/thombashi/pingparsing/actions/workflows/codeql-analysis.yml/badge.svg
-    :target: https://github.com/thombashi/pingparsing/actions/workflows/codeql-analysis.yml
+.. |CodeQL| image:: https://github.com/thombashi/pingparsing/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/pingparsing/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
 CLI Usage
 ====================
 A CLI command (``pingparsing`` command) is included in the package. The command could do the following:
 
 - Execute ``ping`` and parse the result
@@ -525,15 +542,15 @@
 ::
 
     pip install pingparsing
 
 
 Dependencies
 ============
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pingparsing/network/dependencies>`__
 
 Optional Dependencies
 ------------------------------------
 - pingparsing[cli] extras
     - `loguru <https://github.com/Delgan/loguru>`__
         - Used for logging if the package installed
@@ -559,14 +576,16 @@
 +==============+===================================+
 | Ubuntu 16.04 | ``iputils-ping 20121221-5ubuntu2``|
 +--------------+-----------------------------------+
 | Ubuntu 18.04 | ``iputils-ping 20161105-1ubuntu2``|
 +--------------+-----------------------------------+
 | Ubuntu 20.04 | ``iputils-ping 20190709-3``       |
 +--------------+-----------------------------------+
+| Ubuntu 22.04 | ``iputils-ping 20211215-1``       |
++--------------+-----------------------------------+
 | Debian 8.6   | ``iputils-ping 20121221-5+b2``    |
 +--------------+-----------------------------------+
 | Fedora 25    | ``iputils-20161105-1.fc25.x86_64``|
 +--------------+-----------------------------------+
 | Windows 10   | ``-``                             |
 +--------------+-----------------------------------+
 | macOS 10.13  | ``-``                             |
@@ -580,19 +599,27 @@
 
 Documentation
 ===============
 https://pingparsing.rtfd.io/
 
 Sponsors
 ====================================
-.. image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
+|chasbecker| |shiguredo| |b4tman| |Arturi0| |github|
+
+.. |chasbecker| image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
    :target: https://github.com/chasbecker
-   :alt: Charles Becker (chasbecker)
-.. image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
-   :target: https://github.com/Arturi0
-   :alt: onetime: Arturi0
-.. image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
+   :alt: ex-sponsor: Charles Becker (chasbecker)
+.. |shiguredo| image:: https://avatars.githubusercontent.com/u/2549434?s=48&v=4
+   :target: https://github.com/shiguredo
+   :alt: ex-sponsor: 時雨堂 (shiguredo)
+.. |b4tman| image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
    :target: https://github.com/b4tman
    :alt: onetime: Dmitry Belyaev (b4tman)
+.. |Arturi0| image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
+   :target: https://github.com/Arturi0
+   :alt: onetime: Arturi0
+.. |github| image:: https://avatars.githubusercontent.com/u/9919?s=48&v=4
+   :target: https://github.com/github
+   :alt: onetime: GitHub (github)
 
 `Become a sponsor <https://github.com/sponsors/thombashi>`__
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pingparsing-1.4.1/setup.py` & `pingparsing-1.4.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import os.path
-from typing import Dict
+from typing import Dict, Type
 
 import setuptools
 
 
 MODULE_NAME = "pingparsing"
 REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 REQUIREMENT_DIR = "requirements"
 ENCODING = "utf8"
 
 pkg_info: Dict[str, str] = {}
 
 
-def get_release_command_class() -> Dict[str, setuptools.Command]:
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
 
@@ -36,64 +36,72 @@
 
 with open(os.path.join(REQUIREMENT_DIR, "requirements.txt")) as f:
     install_requires = [line.strip() for line in f if line.strip()]
 
 with open(os.path.join(REQUIREMENT_DIR, "test_requirements.txt")) as f:
     tests_requires = [line.strip() for line in f if line.strip()]
 
+with open(os.path.join(REQUIREMENT_DIR, "docs_requirements.txt")) as f:
+    docs_requires = [line.strip() for line in f if line.strip()]
+
 CLI_OPT_REQUIRES = [
     "loguru>=0.4.1,<1",
     "Pygments>=2.1,<3",
 ]
 
 setuptools.setup(
     name=MODULE_NAME,
-    version=pkg_info["__version__"],
     url=REPOSITORY_URL,
     author=pkg_info["__author__"],
     author_email=pkg_info["__email__"],
     description=summary,
     include_package_data=True,
     keywords=["cli", "library", "network", "ping", "parser", "transmitter"],
     license=pkg_info["__license__"],
     long_description=long_description,
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["test*"]),
     package_data={MODULE_NAME: ["py.typed"]},
     project_urls={
+        "Changelog": f"{REPOSITORY_URL:s}/blob/master/CHANGELOG.md",
         "Documentation": f"https://{MODULE_NAME:s}.rtfd.io/",
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
     },
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=install_requires,
-    extras_require={"test": tests_requires, "cli": CLI_OPT_REQUIRES},
+    extras_require={
+        "docs": docs_requires,
+        "test": tests_requires,
+        "cli": CLI_OPT_REQUIRES,
+    },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Telecommunications Industry",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: System :: Networking",
         "Topic :: System :: Networking :: Monitoring",
         "Topic :: Text Processing",
+        "Typing :: Typed",
     ],
     cmdclass=get_release_command_class(),
     entry_points={"console_scripts": ["pingparsing=pingparsing.__main__:main"]},
 )
```

### Comparing `pingparsing-1.4.1/test/data.py` & `pingparsing-1.4.2/test/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -276,29 +276,77 @@
         "packet_duplicate_rate": None,
         "rtt_min": 56,
         "rtt_avg": 107,
         "rtt_max": 194,
         "rtt_mdev": None,
     },
     [
-        {"bytes": 32, "destination": "216.58.196.238", "ttl": 51, "time": 87.0, "duplicate": False},
-        {"bytes": 32, "destination": "216.58.196.238", "ttl": 51, "time": 97.0, "duplicate": False},
-        {"bytes": 32, "destination": "216.58.196.238", "ttl": 51, "time": 56.0, "duplicate": False},
-        {"bytes": 32, "destination": "216.58.196.238", "ttl": 51, "time": 95.0, "duplicate": False},
+        {
+            "bytes": 32,
+            "destination": "216.58.196.238",
+            "ttl": 51,
+            "time": 87.0,
+            "duplicate": False,
+        },
+        {
+            "bytes": 32,
+            "destination": "216.58.196.238",
+            "ttl": 51,
+            "time": 97.0,
+            "duplicate": False,
+        },
+        {
+            "bytes": 32,
+            "destination": "216.58.196.238",
+            "ttl": 51,
+            "time": 56.0,
+            "duplicate": False,
+        },
+        {
+            "bytes": 32,
+            "destination": "216.58.196.238",
+            "ttl": 51,
+            "time": 95.0,
+            "duplicate": False,
+        },
         {
             "bytes": 32,
             "destination": "216.58.196.238",
             "ttl": 51,
             "time": 194.0,
             "duplicate": False,
         },
-        {"bytes": 32, "destination": "216.58.196.238", "ttl": 51, "time": 98.0, "duplicate": False},
-        {"bytes": 32, "destination": "216.58.196.238", "ttl": 51, "time": 93.0, "duplicate": False},
-        {"bytes": 32, "destination": "216.58.196.238", "ttl": 51, "time": 96.0, "duplicate": False},
-        {"bytes": 32, "destination": "216.58.196.238", "ttl": 51, "time": 96.0, "duplicate": False},
+        {
+            "bytes": 32,
+            "destination": "216.58.196.238",
+            "ttl": 51,
+            "time": 98.0,
+            "duplicate": False,
+        },
+        {
+            "bytes": 32,
+            "destination": "216.58.196.238",
+            "ttl": 51,
+            "time": 93.0,
+            "duplicate": False,
+        },
+        {
+            "bytes": 32,
+            "destination": "216.58.196.238",
+            "ttl": 51,
+            "time": 96.0,
+            "duplicate": False,
+        },
+        {
+            "bytes": 32,
+            "destination": "216.58.196.238",
+            "ttl": 51,
+            "time": 96.0,
+            "duplicate": False,
+        },
         {
             "bytes": 32,
             "destination": "216.58.196.238",
             "ttl": 51,
             "time": 165.0,
             "duplicate": False,
         },
```

### Comparing `pingparsing-1.4.1/test/test_cli.py` & `pingparsing-1.4.2/test/test_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,22 +27,24 @@
         tmp_ping_file.write(DEBIAN_SUCCESS_0.value)
         tmp_ping_path = str(tmp_ping_file)
 
         runner = SubprocessRunner([sys.executable, "-m", "pingparsing", tmp_ping_path])
         runner.run()
         print_result(stdout=runner.stdout, stderr=runner.stderr)
         assert runner.returncode == 0
+        assert runner.stdout is not None
         assert json.loads(runner.stdout)[tmp_ping_path] == DEBIAN_SUCCESS_0.expected
 
         runner = SubprocessRunner(
             [sys.executable, "-m", "pingparsing", tmp_ping_path, "--no-color"]
         )
         runner.run()
         print_result(stdout=runner.stdout, stderr=runner.stderr)
         assert runner.returncode == 0
+        assert runner.stdout is not None
         assert json.loads(runner.stdout)[tmp_ping_path] == DEBIAN_SUCCESS_0.expected
 
     def test_normal_multi(self, tmpdir):
         tmp_ping_file_deb = tmpdir.join("ping_deb.txt")
         tmp_ping_file_deb.write(DEBIAN_SUCCESS_0.value)
         tmp_ping_path_deb = str(tmp_ping_file_deb)
 
@@ -54,15 +56,15 @@
             [sys.executable, "-m", "pingparsing", tmp_ping_path_deb, tmp_ping_path_win]
         )
         runner.run()
 
         print_result(stdout=runner.stdout, stderr=runner.stderr)
 
         assert runner.returncode == 0
-
+        assert runner.stdout is not None
         parsed_result = json.loads(runner.stdout)
         assert parsed_result[tmp_ping_path_deb] == DEBIAN_SUCCESS_0.expected
         assert parsed_result[tmp_ping_path_win] == WINDOWS7SP1_SUCCESS.expected
 
     def test_normal_timezone(self, tmpdir):
         tmp_ping_file = tmpdir.join("ping_timezone.txt")
         tmp_ping_file.write(UBUNTU_SUCCESS_1.value)
@@ -78,14 +80,15 @@
                 "UTC",
                 "--no-color",
                 tmp_ping_path,
             ]
         )
         runner.run()
         print_result(stdout=runner.stdout, stderr=runner.stderr)
+        assert runner.stdout is not None
         assert runner.returncode == 0
         assert json.loads(runner.stdout)[tmp_ping_path] == {
             "destination": "google.com",
             "packet_transmit": 5,
             "packet_receive": 5,
             "packet_loss_count": 0,
             "packet_loss_rate": 0.0,
@@ -150,14 +153,15 @@
     def test_normal(self):
         runner = SubprocessRunner([sys.executable, "-m", "pingparsing"])
         runner.run(input=DEBIAN_SUCCESS_0.value)
 
         print_result(stdout=runner.stdout, stderr=runner.stderr)
 
         assert runner.returncode == 0
+        assert runner.stdout is not None
         assert json.loads(runner.stdout) == DEBIAN_SUCCESS_0.expected
 
     def test_normal_w_option(self):
         expected = dedent(
             """\
             {
                 "destination": "google.com",
@@ -202,45 +206,47 @@
         )
         runner = SubprocessRunner([sys.executable, "-m", "pingparsing", "-", "--icmp-reply"])
         runner.run(input=UBUNTU_SUCCESS_2.value)
 
         print_result(stdout=runner.stdout, stderr=runner.stderr, expected=expected)
 
         assert runner.returncode == 0
+        assert runner.stdout is not None
         assert json.loads(runner.stdout) == json.loads(expected)
 
 
 @pytest.mark.xfail(run=False)
 class Test_PingParsing_ping:
     def test_normal_single(self):
         count = 1
         dest = "localhost"
-        runner = SubprocessRunner([sys.executable, "-m", "pingparsing", dest, "-c", count])
+        runner = SubprocessRunner([sys.executable, "-m", "pingparsing", dest, "-c", str(count)])
         runner.run()
 
         print_result(stdout=runner.stdout, stderr=runner.stderr)
 
         assert runner.returncode == 0
-
+        assert runner.stdout is not None
         parsed_result = json.loads(runner.stdout)
-
         assert parsed_result[dest]["packet_transmit"] == count
         assert parsed_result[dest]["rtt_max"] > 0
 
     def test_normal_multi(self):
         count = 1
         dest_list = ["google.com", "twitter.com"]
-        runner = SubprocessRunner([sys.executable, "-m", "pingparsing"] + dest_list + ["-c", count])
+        runner = SubprocessRunner(
+            [sys.executable, "-m", "pingparsing"] + dest_list + ["-c", str(count)]
+        )
         print(runner.command_str, file=sys.stderr)
         runner.run()
 
         print_result(stdout=runner.stdout, stderr=runner.stderr)
 
         assert runner.returncode == 0
-
+        assert runner.stdout is not None
         parsed_result = json.loads(runner.stdout)
         for dest in dest_list:
             assert parsed_result[dest]["packet_transmit"] == count
             assert parsed_result[dest]["rtt_max"] > 0
 
     def test_normal_single_icmp_timestamp(self):
         count = 1
@@ -248,26 +254,26 @@
         runner = SubprocessRunner(
             [
                 sys.executable,
                 "-m",
                 "pingparsing",
                 dest,
                 "-c",
-                count,
+                str(count),
                 "--icmp-reply",
                 "--timestamp",
                 "epoch",
             ]
         )
         runner.run()
 
         print_result(stdout=runner.stdout, stderr=runner.stderr)
 
         assert runner.returncode == 0
-
+        assert runner.stdout is not None
         parsed_result = json.loads(runner.stdout)
 
         assert parsed_result[dest]["packet_transmit"] == count
         assert parsed_result[dest]["rtt_max"] > 0
 
         icmp_replies = parsed_result[dest]["icmp_replies"]
         assert icmp_replies
```

### Comparing `pingparsing-1.4.1/test/test_cmd_maker.py` & `pingparsing-1.4.2/test/test_cmd_maker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-
 import pytest
 from humanreadable import Time
 
 from pingparsing._cmd_maker import LinuxPingCmdMaker, MacosPingCmdMaker, WindowsPingCmdMaker
 
 
 class Test_CmdMaker_make_cmd:
@@ -43,16 +42,28 @@
             [
                 LinuxPingCmdMaker,
                 "localhost",
                 True,
                 "1sec",
                 "ping6 -I eth0 -w 3 -W 1 localhost".split(),
             ],
-            [MacosPingCmdMaker, "localhost", False, "1sec", "ping -t 3 localhost".split()],
-            [MacosPingCmdMaker, "localhost", True, "1sec", "ping6 -i 1 -c 3 localhost".split()],
+            [
+                MacosPingCmdMaker,
+                "localhost",
+                False,
+                "1sec",
+                "ping -t 3 localhost".split(),
+            ],
+            [
+                MacosPingCmdMaker,
+                "localhost",
+                True,
+                "1sec",
+                "ping6 -i 1 -c 3 localhost".split(),
+            ],
             [
                 WindowsPingCmdMaker,
                 "localhost",
                 False,
                 "1sec",
                 "ping -n 3 -w 1000 localhost".split(),
             ],
@@ -83,17 +94,32 @@
     )
     def test_normal_count(self, maker_class, host, count, expected):
         assert maker_class(count=count).make_cmd(destination=host) == expected
 
     @pytest.mark.parametrize(
         ["maker_class", "host", "packet_size", "expected"],
         [
-            [LinuxPingCmdMaker, "localhost", 6000, "ping -c 1 -s 6000 localhost".split()],
-            [MacosPingCmdMaker, "localhost", 6000, "ping -c 1 -s 6000 localhost".split()],
-            [WindowsPingCmdMaker, "localhost", 6000, "ping -n 1 -l 6000 localhost".split()],
+            [
+                LinuxPingCmdMaker,
+                "localhost",
+                6000,
+                "ping -c 1 -s 6000 localhost".split(),
+            ],
+            [
+                MacosPingCmdMaker,
+                "localhost",
+                6000,
+                "ping -c 1 -s 6000 localhost".split(),
+            ],
+            [
+                WindowsPingCmdMaker,
+                "localhost",
+                6000,
+                "ping -n 1 -l 6000 localhost".split(),
+            ],
         ],
     )
     def test_normal_packet_size(self, maker_class, host, packet_size, expected):
         assert maker_class(packet_size=packet_size, count=1).make_cmd(destination=host) == expected
 
     @pytest.mark.parametrize(
         ["maker_class", "host", "ttl", "expected"],
```

### Comparing `pingparsing-1.4.1/test/test_logger.py` & `pingparsing-1.4.2/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `pingparsing-1.4.1/test/test_pingparsing.py` & `pingparsing-1.4.2/test/test_pingparsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from textwrap import dedent
 
 import pytest
 import pytz
 
 from pingparsing import ParseError, PingResult
 
-from .common import PingTestData, ping_parser  # noqa: W0611
+from .common import PingTestData, ping_parser  # noqa
 from .data import (
     DEBIAN_SUCCESS_0,
     UBUNTU_SUCCESS_0,
     UBUNTU_SUCCESS_1,
     UBUNTU_SUCCESS_2,
     WINDOWS7SP1_SUCCESS,
 )
@@ -672,23 +672,77 @@
         "packet_duplicate_rate": None,
         "rtt_min": 0.0,
         "rtt_avg": 14.0,
         "rtt_max": 33.0,
         "rtt_mdev": None,
     },
     [
-        {"bytes": 32, "destination": "192.168.2.106", "ttl": 64, "time": 16.0, "duplicate": False},
-        {"bytes": 32, "destination": "192.168.2.106", "ttl": 64, "time": 6.0, "duplicate": False},
-        {"bytes": 32, "destination": "192.168.2.106", "ttl": 64, "time": 12.0, "duplicate": False},
-        {"bytes": 32, "destination": "192.168.2.106", "ttl": 64, "time": 16.0, "duplicate": False},
-        {"bytes": 32, "destination": "192.168.2.106", "ttl": 64, "time": 8.0, "duplicate": False},
-        {"bytes": 32, "destination": "192.168.2.106", "ttl": 64, "time": 33.0, "duplicate": False},
-        {"bytes": 32, "destination": "192.168.2.106", "ttl": 64, "time": 13.0, "duplicate": False},
-        {"bytes": 32, "destination": "192.168.2.106", "ttl": 64, "time": 23.0, "duplicate": False},
-        {"bytes": 32, "destination": "192.168.2.106", "ttl": 64, "time": 1.0, "duplicate": False},
+        {
+            "bytes": 32,
+            "destination": "192.168.2.106",
+            "ttl": 64,
+            "time": 16.0,
+            "duplicate": False,
+        },
+        {
+            "bytes": 32,
+            "destination": "192.168.2.106",
+            "ttl": 64,
+            "time": 6.0,
+            "duplicate": False,
+        },
+        {
+            "bytes": 32,
+            "destination": "192.168.2.106",
+            "ttl": 64,
+            "time": 12.0,
+            "duplicate": False,
+        },
+        {
+            "bytes": 32,
+            "destination": "192.168.2.106",
+            "ttl": 64,
+            "time": 16.0,
+            "duplicate": False,
+        },
+        {
+            "bytes": 32,
+            "destination": "192.168.2.106",
+            "ttl": 64,
+            "time": 8.0,
+            "duplicate": False,
+        },
+        {
+            "bytes": 32,
+            "destination": "192.168.2.106",
+            "ttl": 64,
+            "time": 33.0,
+            "duplicate": False,
+        },
+        {
+            "bytes": 32,
+            "destination": "192.168.2.106",
+            "ttl": 64,
+            "time": 13.0,
+            "duplicate": False,
+        },
+        {
+            "bytes": 32,
+            "destination": "192.168.2.106",
+            "ttl": 64,
+            "time": 23.0,
+            "duplicate": False,
+        },
+        {
+            "bytes": 32,
+            "destination": "192.168.2.106",
+            "ttl": 64,
+            "time": 1.0,
+            "duplicate": False,
+        },
     ],
 )
 WINDOWS_UNREACHABLE_0 = PingTestData(
     dedent(
         """\
         Pinging 192.168.207.100 with 32 bytes of data:
         Request timed out.
@@ -763,15 +817,19 @@
 
         assert ping_parser.parser_name == parser_name
         assert stats.as_dict() == test_data.expected
         assert stats.icmp_replies == test_data.replies
 
     @pytest.mark.xfail(run=False)
     @pytest.mark.parametrize(
-        ["test_data", "parser_name"], [[UBUNTU_SUCCESS_1, "Linux"], [UBUNTU_SUCCESS_2, "Linux"]]
+        ["test_data", "parser_name"],
+        [
+            [UBUNTU_SUCCESS_1, "Linux"],
+            [UBUNTU_SUCCESS_2, "Linux"],
+        ],
     )
     def test_normal_timestamp(self, ping_parser, test_data, parser_name):
         stats = ping_parser.parse(test_data.value)
 
         print(f"[input text]\n{test_data.value}\n")
         print(f"[expected]\n{test_data.expected}\n")
         print(f"[actual]\n{stats.as_dict()}\n")
@@ -812,15 +870,18 @@
     )
     def test_ping_failure(self, ping_parser, value):
         stats = ping_parser.parse(value)
         assert stats.is_empty()
 
     @pytest.mark.parametrize(
         ["value", "expected"],
-        [[PING_FEDORA_EMPTY_BODY, ParseError], [PING_WINDOWS_INVALID, ParseError]],
+        [
+            [PING_FEDORA_EMPTY_BODY, ParseError],
+            [PING_WINDOWS_INVALID, ParseError],
+        ],
     )
     def test_exception(self, ping_parser, value, expected):
         with pytest.raises(expected):
             ping_parser.parse(value)
 
 
 class Test_PingParsing_as_tuple:
```

### Comparing `pingparsing-1.4.1/test/test_pingresult.py` & `pingparsing-1.4.2/test/test_pingresult.py`

 * *Files identical despite different names*

### Comparing `pingparsing-1.4.1/test/test_pingtransmitter.py` & `pingparsing-1.4.2/test/test_pingtransmitter.py`

 * *Files identical despite different names*

### Comparing `pingparsing-1.4.1/tox.ini` & `pingparsing-1.4.2/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 envlist =
-    py{36,37,38,39,310,311}
+    py{37,38,39,310,311,312}
     pypy3
     build
     cov
     docs
     fmt
     readme
 
@@ -12,20 +12,20 @@
 extras =
     test
 commands =
     pytest {posargs}
 
 [testenv:build]
 deps =
+    build>=1
     twine
     wheel
 commands =
-    python setup.py sdist bdist_wheel
+    python -m build
     twine check dist/*.whl dist/*.tar.gz
-    python setup.py clean --all
 
 [testenv:clean]
 skip_install = true
 deps =
     cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
@@ -36,46 +36,63 @@
 deps =
     coverage[toml]>=5
 commands =
     coverage run -m pytest {posargs:-vv}
     coverage report -m
 
 [testenv:docs]
+extras =
+    docs
+commands =
+    sphinx-build docs/ docs/_build
+
+[testenv:fmt-black]
+skip_install = true
 deps =
-    -r{toxinidir}/requirements/docs_requirements.txt
+    autoflake>=2
+    black>=24.1
+    isort>=5
 commands =
-    python setup.py build_sphinx --source-dir=docs/ --build-dir=docs/_build --all-files
+    autoflake --in-place --recursive --remove-all-unused-imports .
+    isort .
+    black setup.py test pingparsing examples
 
 [testenv:fmt]
 skip_install = true
 deps =
     autoflake>=2
-    black>=23.1
     isort>=5
+    ruff>=0.3.5
 commands =
-    autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
+    autoflake --in-place --recursive --remove-all-unused-imports .
     isort .
-    black setup.py test pingparsing examples
+    ruff format
 
 [testenv:lint]
 skip_install = true
 deps =
-    codespell
+    codespell>=2
     mypy>=1
-    pylama>=8.4.1
     types-pytz
     types-simplejson
+    ruff>=0.3.5
 commands =
-    python setup.py check
     codespell pingparsing docs/pages examples test -q 2 --check-filenames
     mypy pingparsing setup.py
-    pylama setup.py examples pingparsing test
+    ruff format --check
+    ruff check
 
 [testenv:readme]
 changedir = docs
 extras =
     cli
 deps =
     path
     readmemaker>=1.1.0
 commands =
     python make_readme.py
+
+[testenv:release]
+deps =
+    releasecmd
+commands =
+    python setup.py release --sign --skip-uploading --verbose
```

