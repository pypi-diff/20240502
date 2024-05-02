# Comparing `tmp/abtoolkit-1.2.5.tar.gz` & `tmp/abtoolkit-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abtoolkit-1.2.5.tar", last modified: Mon Apr 22 11:19:03 2024, max compression
+gzip compressed data, was "abtoolkit-1.2.6.tar", last modified: Thu May  2 14:23:24 2024, max compression
```

## Comparing `abtoolkit-1.2.5.tar` & `abtoolkit-1.2.6.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-22 11:19:03.576591 abtoolkit-1.2.5/
--rw-r--r--   0 naltukhov (1397289063) 359461530       32 2024-03-22 14:05:39.000000 abtoolkit-1.2.5/.gitignore
--rw-r--r--   0 naltukhov (1397289063) 359461530     1062 2024-03-22 09:28:06.000000 abtoolkit-1.2.5/LICENSE
--rw-r--r--   0 naltukhov (1397289063) 359461530      558 2024-03-23 09:48:31.000000 abtoolkit-1.2.5/Makefile
--rw-r--r--   0 naltukhov (1397289063) 359461530     6694 2024-04-22 11:19:03.576321 abtoolkit-1.2.5/PKG-INFO
--rw-r--r--   0 naltukhov (1397289063) 359461530     5964 2024-04-22 11:16:31.000000 abtoolkit-1.2.5/README.md
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-22 11:19:03.559916 abtoolkit-1.2.5/abtoolkit/
--rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-23 05:39:11.000000 abtoolkit-1.2.5/abtoolkit/__init__.py
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-22 11:19:03.561634 abtoolkit-1.2.5/abtoolkit/continuous/
--rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-22 09:33:10.000000 abtoolkit-1.2.5/abtoolkit/continuous/__init__.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     7637 2024-03-29 12:15:29.000000 abtoolkit-1.2.5/abtoolkit/continuous/simulation.py
--rw-r--r--   0 naltukhov (1397289063) 359461530    10878 2024-03-29 13:46:05.000000 abtoolkit-1.2.5/abtoolkit/continuous/stattests.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     3381 2024-03-29 11:44:42.000000 abtoolkit-1.2.5/abtoolkit/continuous/utils.py
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-22 11:19:03.562468 abtoolkit-1.2.5/abtoolkit/discrete/
--rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-22 09:32:58.000000 abtoolkit-1.2.5/abtoolkit/discrete/__init__.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     2396 2024-03-29 12:15:29.000000 abtoolkit-1.2.5/abtoolkit/discrete/simulation.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     1609 2024-03-29 11:46:38.000000 abtoolkit-1.2.5/abtoolkit/discrete/stattests.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     3080 2024-04-19 14:27:08.000000 abtoolkit-1.2.5/abtoolkit/discrete/utils.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     8459 2024-04-22 11:16:53.000000 abtoolkit-1.2.5/abtoolkit/utils.py
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-22 11:19:03.576042 abtoolkit-1.2.5/abtoolkit.egg-info/
--rw-r--r--   0 naltukhov (1397289063) 359461530     6694 2024-04-22 11:19:03.000000 abtoolkit-1.2.5/abtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 naltukhov (1397289063) 359461530     1268 2024-04-22 11:19:03.000000 abtoolkit-1.2.5/abtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 naltukhov (1397289063) 359461530        1 2024-04-22 11:19:03.000000 abtoolkit-1.2.5/abtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 naltukhov (1397289063) 359461530       93 2024-04-22 11:19:03.000000 abtoolkit-1.2.5/abtoolkit.egg-info/requires.txt
--rw-r--r--   0 naltukhov (1397289063) 359461530       42 2024-04-22 11:19:03.000000 abtoolkit-1.2.5/abtoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-22 11:19:03.562962 abtoolkit-1.2.5/examples/
--rw-r--r--   0 naltukhov (1397289063) 359461530     1844 2024-03-29 14:11:25.000000 abtoolkit-1.2.5/examples/continuous_var_analysis.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     1479 2024-03-29 11:34:01.000000 abtoolkit-1.2.5/examples/discrete_var_analysis.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      260 2024-03-23 09:42:57.000000 abtoolkit-1.2.5/pre-commit.bash
--rw-r--r--   0 naltukhov (1397289063) 359461530     1021 2024-04-22 11:18:50.000000 abtoolkit-1.2.5/pyproject.toml
--rw-r--r--   0 naltukhov (1397289063) 359461530      110 2024-03-22 14:16:03.000000 abtoolkit-1.2.5/requirements.txt
--rw-r--r--   0 naltukhov (1397289063) 359461530       38 2024-04-22 11:19:03.576636 abtoolkit-1.2.5/setup.cfg
--rw-r--r--   0 naltukhov (1397289063) 359461530      256 2024-04-19 07:41:47.000000 abtoolkit-1.2.5/setup.py
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-22 11:19:03.568915 abtoolkit-1.2.5/static/
--rw-r--r--   0 naltukhov (1397289063) 359461530    41812 2024-03-29 12:49:51.000000 abtoolkit-1.2.5/static/discrete-output-plot.png
--rw-r--r--   0 naltukhov (1397289063) 359461530   135844 2024-03-29 12:50:41.000000 abtoolkit-1.2.5/static/discrete-p-value-plot.png
--rw-r--r--   0 naltukhov (1397289063) 359461530   185112 2024-03-29 12:52:31.000000 abtoolkit-1.2.5/static/output-plot.png
--rw-r--r--   0 naltukhov (1397289063) 359461530   205019 2024-03-22 08:45:06.000000 abtoolkit-1.2.5/static/p-value-plot.png
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-22 11:19:03.572347 abtoolkit-1.2.5/tests/
--rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-22 08:45:06.000000 abtoolkit-1.2.5/tests/__init__.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     2727 2024-03-29 08:48:35.000000 abtoolkit-1.2.5/tests/test_continuous_simulation.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     5436 2024-03-29 08:48:35.000000 abtoolkit-1.2.5/tests/test_continuous_stattests.py
--rw-r--r--   0 naltukhov (1397289063) 359461530      795 2024-03-25 10:43:06.000000 abtoolkit-1.2.5/tests/test_continuous_utils.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     2426 2024-03-29 10:20:21.000000 abtoolkit-1.2.5/tests/test_discrete_simulation.py
--rw-r--r--   0 naltukhov (1397289063) 359461530      583 2024-03-29 09:29:26.000000 abtoolkit-1.2.5/tests/test_discrete_stattests.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     1220 2024-04-19 14:24:13.000000 abtoolkit-1.2.5/tests/test_discrete_utils.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     1427 2024-04-22 11:17:28.000000 abtoolkit-1.2.5/tests/test_utils.py
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-22 11:19:03.557831 abtoolkit-1.2.5/venv/
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-22 11:19:03.575734 abtoolkit-1.2.5/venv/bin/
--rw-r--r--   0 naltukhov (1397289063) 359461530     1175 2024-03-22 08:53:42.000000 abtoolkit-1.2.5/venv/bin/activate_this.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      648 2024-03-22 14:05:07.000000 abtoolkit-1.2.5/venv/bin/rst2html.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      770 2024-03-22 14:05:07.000000 abtoolkit-1.2.5/venv/bin/rst2html4.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530     1105 2024-03-22 14:05:07.000000 abtoolkit-1.2.5/venv/bin/rst2html5.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      847 2024-03-22 14:05:07.000000 abtoolkit-1.2.5/venv/bin/rst2latex.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      670 2024-03-22 14:05:07.000000 abtoolkit-1.2.5/venv/bin/rst2man.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      836 2024-03-22 14:05:07.000000 abtoolkit-1.2.5/venv/bin/rst2odt.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      642 2024-03-22 14:05:07.000000 abtoolkit-1.2.5/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      655 2024-03-22 14:05:07.000000 abtoolkit-1.2.5/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      691 2024-03-22 14:05:07.000000 abtoolkit-1.2.5/venv/bin/rst2s5.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      927 2024-03-22 14:05:07.000000 abtoolkit-1.2.5/venv/bin/rst2xetex.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      656 2024-03-22 14:05:07.000000 abtoolkit-1.2.5/venv/bin/rst2xml.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      724 2024-03-22 14:05:07.000000 abtoolkit-1.2.5/venv/bin/rstpep2html.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-05-02 14:23:24.491560 abtoolkit-1.2.6/
+-rw-r--r--   0 naltukhov (1397289063) 359461530       32 2024-03-22 14:05:39.000000 abtoolkit-1.2.6/.gitignore
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1062 2024-03-22 09:28:06.000000 abtoolkit-1.2.6/LICENSE
+-rw-r--r--   0 naltukhov (1397289063) 359461530      558 2024-03-23 09:48:31.000000 abtoolkit-1.2.6/Makefile
+-rw-r--r--   0 naltukhov (1397289063) 359461530     6694 2024-05-02 14:23:24.491332 abtoolkit-1.2.6/PKG-INFO
+-rw-r--r--   0 naltukhov (1397289063) 359461530     5964 2024-04-22 11:16:31.000000 abtoolkit-1.2.6/README.md
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-05-02 14:23:24.474660 abtoolkit-1.2.6/abtoolkit/
+-rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-23 05:39:11.000000 abtoolkit-1.2.6/abtoolkit/__init__.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-05-02 14:23:24.475950 abtoolkit-1.2.6/abtoolkit/continuous/
+-rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-22 09:33:10.000000 abtoolkit-1.2.6/abtoolkit/continuous/__init__.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     7637 2024-03-29 12:15:29.000000 abtoolkit-1.2.6/abtoolkit/continuous/simulation.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530    10878 2024-03-29 13:46:05.000000 abtoolkit-1.2.6/abtoolkit/continuous/stattests.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     3381 2024-03-29 11:44:42.000000 abtoolkit-1.2.6/abtoolkit/continuous/utils.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-05-02 14:23:24.476435 abtoolkit-1.2.6/abtoolkit/discrete/
+-rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-22 09:32:58.000000 abtoolkit-1.2.6/abtoolkit/discrete/__init__.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     2396 2024-03-29 12:15:29.000000 abtoolkit-1.2.6/abtoolkit/discrete/simulation.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1609 2024-03-29 11:46:38.000000 abtoolkit-1.2.6/abtoolkit/discrete/stattests.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     3080 2024-04-19 14:27:08.000000 abtoolkit-1.2.6/abtoolkit/discrete/utils.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     8446 2024-05-02 14:08:37.000000 abtoolkit-1.2.6/abtoolkit/utils.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-05-02 14:23:24.491045 abtoolkit-1.2.6/abtoolkit.egg-info/
+-rw-r--r--   0 naltukhov (1397289063) 359461530     6694 2024-05-02 14:23:24.000000 abtoolkit-1.2.6/abtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1290 2024-05-02 14:23:24.000000 abtoolkit-1.2.6/abtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 naltukhov (1397289063) 359461530        1 2024-05-02 14:23:24.000000 abtoolkit-1.2.6/abtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 naltukhov (1397289063) 359461530       93 2024-05-02 14:23:24.000000 abtoolkit-1.2.6/abtoolkit.egg-info/requires.txt
+-rw-r--r--   0 naltukhov (1397289063) 359461530       42 2024-05-02 14:23:24.000000 abtoolkit-1.2.6/abtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-05-02 14:23:24.477333 abtoolkit-1.2.6/examples/
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1064 2024-05-02 14:21:23.000000 abtoolkit-1.2.6/examples/check_clt.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1844 2024-03-29 14:11:25.000000 abtoolkit-1.2.6/examples/continuous_var_analysis.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1479 2024-03-29 11:34:01.000000 abtoolkit-1.2.6/examples/discrete_var_analysis.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      260 2024-03-23 09:42:57.000000 abtoolkit-1.2.6/pre-commit.bash
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1021 2024-05-02 14:23:05.000000 abtoolkit-1.2.6/pyproject.toml
+-rw-r--r--   0 naltukhov (1397289063) 359461530      110 2024-03-22 14:16:03.000000 abtoolkit-1.2.6/requirements.txt
+-rw-r--r--   0 naltukhov (1397289063) 359461530       38 2024-05-02 14:23:24.491607 abtoolkit-1.2.6/setup.cfg
+-rw-r--r--   0 naltukhov (1397289063) 359461530      256 2024-04-19 07:41:47.000000 abtoolkit-1.2.6/setup.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-05-02 14:23:24.483687 abtoolkit-1.2.6/static/
+-rw-r--r--   0 naltukhov (1397289063) 359461530    41812 2024-03-29 12:49:51.000000 abtoolkit-1.2.6/static/discrete-output-plot.png
+-rw-r--r--   0 naltukhov (1397289063) 359461530   135844 2024-03-29 12:50:41.000000 abtoolkit-1.2.6/static/discrete-p-value-plot.png
+-rw-r--r--   0 naltukhov (1397289063) 359461530   185112 2024-03-29 12:52:31.000000 abtoolkit-1.2.6/static/output-plot.png
+-rw-r--r--   0 naltukhov (1397289063) 359461530   205019 2024-03-22 08:45:06.000000 abtoolkit-1.2.6/static/p-value-plot.png
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-05-02 14:23:24.486897 abtoolkit-1.2.6/tests/
+-rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-22 08:45:06.000000 abtoolkit-1.2.6/tests/__init__.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     2727 2024-03-29 08:48:35.000000 abtoolkit-1.2.6/tests/test_continuous_simulation.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     5436 2024-03-29 08:48:35.000000 abtoolkit-1.2.6/tests/test_continuous_stattests.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530      795 2024-03-25 10:43:06.000000 abtoolkit-1.2.6/tests/test_continuous_utils.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     2426 2024-03-29 10:20:21.000000 abtoolkit-1.2.6/tests/test_discrete_simulation.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530      583 2024-03-29 09:29:26.000000 abtoolkit-1.2.6/tests/test_discrete_stattests.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1220 2024-04-19 14:24:13.000000 abtoolkit-1.2.6/tests/test_discrete_utils.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1411 2024-05-02 14:06:52.000000 abtoolkit-1.2.6/tests/test_utils.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-05-02 14:23:24.472516 abtoolkit-1.2.6/venv/
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-05-02 14:23:24.490727 abtoolkit-1.2.6/venv/bin/
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1175 2024-03-22 08:53:42.000000 abtoolkit-1.2.6/venv/bin/activate_this.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      648 2024-03-22 14:05:07.000000 abtoolkit-1.2.6/venv/bin/rst2html.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      770 2024-03-22 14:05:07.000000 abtoolkit-1.2.6/venv/bin/rst2html4.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530     1105 2024-03-22 14:05:07.000000 abtoolkit-1.2.6/venv/bin/rst2html5.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      847 2024-03-22 14:05:07.000000 abtoolkit-1.2.6/venv/bin/rst2latex.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      670 2024-03-22 14:05:07.000000 abtoolkit-1.2.6/venv/bin/rst2man.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      836 2024-03-22 14:05:07.000000 abtoolkit-1.2.6/venv/bin/rst2odt.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      642 2024-03-22 14:05:07.000000 abtoolkit-1.2.6/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      655 2024-03-22 14:05:07.000000 abtoolkit-1.2.6/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      691 2024-03-22 14:05:07.000000 abtoolkit-1.2.6/venv/bin/rst2s5.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      927 2024-03-22 14:05:07.000000 abtoolkit-1.2.6/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      656 2024-03-22 14:05:07.000000 abtoolkit-1.2.6/venv/bin/rst2xml.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      724 2024-03-22 14:05:07.000000 abtoolkit-1.2.6/venv/bin/rstpep2html.py
```

### Comparing `abtoolkit-1.2.5/LICENSE` & `abtoolkit-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/Makefile` & `abtoolkit-1.2.6/Makefile`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/PKG-INFO` & `abtoolkit-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abtoolkit
-Version: 1.2.5
+Version: 1.2.6
 Summary: Package with tools for AB testing
 Author-email: Nikita Altukhov <altuxov.nikita@gmail.com>
 Project-URL: Homepage, https://github.com/nikitosl/abtoolkit
 Project-URL: Issues, https://github.com/nikitosl/abtoolkit/issues
 Keywords: ab_test,cuped,did,ttest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abtoolkit-1.2.5/README.md` & `abtoolkit-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/abtoolkit/continuous/simulation.py` & `abtoolkit-1.2.6/abtoolkit/continuous/simulation.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/abtoolkit/continuous/stattests.py` & `abtoolkit-1.2.6/abtoolkit/continuous/stattests.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/abtoolkit/continuous/utils.py` & `abtoolkit-1.2.6/abtoolkit/continuous/utils.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/abtoolkit/discrete/simulation.py` & `abtoolkit-1.2.6/abtoolkit/discrete/simulation.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/abtoolkit/discrete/stattests.py` & `abtoolkit-1.2.6/abtoolkit/discrete/stattests.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/abtoolkit/discrete/utils.py` & `abtoolkit-1.2.6/abtoolkit/discrete/utils.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/abtoolkit/utils.py` & `abtoolkit-1.2.6/abtoolkit/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,39 +13,39 @@
 
 from abtoolkit.discrete.utils import estimate_ci_binomial
 
 
 def check_clt(
     variable,
     do_plot_distribution: bool = True,
-    sampling_length: int = None,
-    simulations_num: int = 5000,
+    sample_size: int = None,
+    experiments_num: int = 5000,
     metric_f: Callable[[List, any], float] = np.mean,
     **metric_f_kwargs,
 ) -> float:
     """
-    Tests the central limit theorem by sampling subsamples of length `sampling_length`, `simulations_num` times.
+    Tests the central limit theorem by sampling subsamples of length `sample_size`, `experiments_num` times.
     `metric_f` is then taken from a subsample and the distribution of such values is compared to the normal
     distribution using the Shapiro-Wilk test. Returns p-value, where the null hypothesis that the weights were drawn
     from a normal distribution and alternative is another distribution. So if p-value lower 0.05 then variable doesn't
     consider CLT.
     :param variable: array-like, variable we want to test
-    :param sampling_length: subsample size we take on each simulation step, if None then take length(variable).
+    :param sample_size: subsample size we take on each simulation step, if None then take length(variable).
     Default = None
-    :param simulations_num: number of simulations, default = 5000
+    :param experiments_num: number of simulations for estimation, default = 5000
     :param metric_f: function to take from subsample, default = numpy.mean(). Additional args could be given using
     metric_kwargs parameter
     :param do_plot_distribution: whether to plot distribution or not, default = True
     :return: p-value of Shapiro-Wilk test for normality
     """
 
-    sampling_length = len(variable) if sampling_length is None else sampling_length
+    sample_size = len(variable) if sample_size is None else sample_size
     values = []
-    for _ in tqdm(range(simulations_num)):
-        sample = np.random.choice(variable, size=sampling_length, replace=True)
+    for _ in tqdm(range(experiments_num)):
+        sample = np.random.choice(variable, size=sample_size, replace=True)
         values.append(metric_f(sample, **metric_f_kwargs))
 
     # Shapiro-Wilk test
     res = shapiro(values)
 
     if do_plot_distribution:
         plt.hist(values, bins=100)
```

### Comparing `abtoolkit-1.2.5/abtoolkit.egg-info/PKG-INFO` & `abtoolkit-1.2.6/abtoolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abtoolkit
-Version: 1.2.5
+Version: 1.2.6
 Summary: Package with tools for AB testing
 Author-email: Nikita Altukhov <altuxov.nikita@gmail.com>
 Project-URL: Homepage, https://github.com/nikitosl/abtoolkit
 Project-URL: Issues, https://github.com/nikitosl/abtoolkit/issues
 Keywords: ab_test,cuped,did,ttest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abtoolkit-1.2.5/abtoolkit.egg-info/SOURCES.txt` & `abtoolkit-1.2.6/abtoolkit.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 abtoolkit/continuous/simulation.py
 abtoolkit/continuous/stattests.py
 abtoolkit/continuous/utils.py
 abtoolkit/discrete/__init__.py
 abtoolkit/discrete/simulation.py
 abtoolkit/discrete/stattests.py
 abtoolkit/discrete/utils.py
+examples/check_clt.py
 examples/continuous_var_analysis.py
 examples/discrete_var_analysis.py
 static/discrete-output-plot.png
 static/discrete-p-value-plot.png
 static/output-plot.png
 static/p-value-plot.png
 tests/__init__.py
```

### Comparing `abtoolkit-1.2.5/examples/continuous_var_analysis.py` & `abtoolkit-1.2.6/examples/continuous_var_analysis.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/examples/discrete_var_analysis.py` & `abtoolkit-1.2.6/examples/discrete_var_analysis.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/pyproject.toml` & `abtoolkit-1.2.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "abtoolkit"
-version = "1.2.5"
+version = "1.2.6"
 authors = [
   { name="Nikita Altukhov", email="altuxov.nikita@gmail.com" },
 ]
 description = "Package with tools for AB testing"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `abtoolkit-1.2.5/static/discrete-output-plot.png` & `abtoolkit-1.2.6/static/discrete-output-plot.png`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/static/discrete-p-value-plot.png` & `abtoolkit-1.2.6/static/discrete-p-value-plot.png`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/static/output-plot.png` & `abtoolkit-1.2.6/static/output-plot.png`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/static/p-value-plot.png` & `abtoolkit-1.2.6/static/p-value-plot.png`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/tests/test_continuous_simulation.py` & `abtoolkit-1.2.6/tests/test_continuous_simulation.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/tests/test_continuous_stattests.py` & `abtoolkit-1.2.6/tests/test_continuous_stattests.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/tests/test_continuous_utils.py` & `abtoolkit-1.2.6/tests/test_continuous_utils.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/tests/test_discrete_simulation.py` & `abtoolkit-1.2.6/tests/test_discrete_simulation.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/tests/test_discrete_stattests.py` & `abtoolkit-1.2.6/tests/test_discrete_stattests.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/tests/test_discrete_utils.py` & `abtoolkit-1.2.6/tests/test_discrete_utils.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/tests/test_utils.py` & `abtoolkit-1.2.6/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 import numpy as np
 from abtoolkit.utils import check_clt
 
 
 class TestUtils(unittest.TestCase):
     def test_check_central_limit_theorem_normal(self):
         var = np.random.normal(0, 2, size=10000)
-        p_value = check_clt(var, do_plot_distribution=False, sampling_length=10)
+        p_value = check_clt(var, do_plot_distribution=False, sample_size=10)
         self.assertTrue(p_value >= 0, f"p-value: {p_value}")
 
     def test_check_central_limit_theorem_continuous(self):
         var = np.random.chisquare(df=2, size=10000)
-        p_value = check_clt(var, do_plot_distribution=False, sampling_length=10000)
+        p_value = check_clt(var, do_plot_distribution=False, sample_size=10000)
         self.assertTrue(p_value >= 0, f"p-value: {p_value}")
 
     def test_check_central_limit_theorem_discrete(self):
         var = np.random.choice([0, 1], p=[0.93, 0.07], size=10000)
-        p_value = check_clt(var, do_plot_distribution=False, sampling_length=50000)
+        p_value = check_clt(var, do_plot_distribution=False, sample_size=50000)
         self.assertTrue(p_value >= 0, f"p-value: {p_value}")
 
     def test_check_central_limit_theorem_normal_median(self):
         var = np.random.normal(0, 2, size=10000)
-        p_value = check_clt(var, do_plot_distribution=False, sampling_length=10, metric_f=np.median)
+        p_value = check_clt(var, do_plot_distribution=False, sample_size=10, metric_f=np.median)
         self.assertTrue(p_value >= 0, f"p-value: {p_value}")
 
     def test_check_central_limit_theorem_normal_percentile(self):
         var = np.random.normal(0, 2, size=10000)
         p_value = check_clt(var, do_plot_distribution=False, metric_f=np.percentile, q=0.9)
         self.assertTrue(p_value >= 0, f"p-value: {p_value}")
```

### Comparing `abtoolkit-1.2.5/venv/bin/activate_this.py` & `abtoolkit-1.2.6/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/venv/bin/rst2html.py` & `abtoolkit-1.2.6/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/venv/bin/rst2html4.py` & `abtoolkit-1.2.6/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/venv/bin/rst2html5.py` & `abtoolkit-1.2.6/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/venv/bin/rst2latex.py` & `abtoolkit-1.2.6/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/venv/bin/rst2man.py` & `abtoolkit-1.2.6/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/venv/bin/rst2odt.py` & `abtoolkit-1.2.6/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/venv/bin/rst2odt_prepstyles.py` & `abtoolkit-1.2.6/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/venv/bin/rst2pseudoxml.py` & `abtoolkit-1.2.6/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/venv/bin/rst2s5.py` & `abtoolkit-1.2.6/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/venv/bin/rst2xetex.py` & `abtoolkit-1.2.6/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/venv/bin/rst2xml.py` & `abtoolkit-1.2.6/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.5/venv/bin/rstpep2html.py` & `abtoolkit-1.2.6/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

