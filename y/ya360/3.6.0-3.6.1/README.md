# Comparing `tmp/ya360-3.6.0.tar.gz` & `tmp/ya360-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ya360-3.6.0.tar", last modified: Fri Apr  5 07:28:42 2024, max compression
+gzip compressed data, was "ya360-3.6.1.tar", last modified: Thu May  2 10:25:36 2024, max compression
```

## Comparing `ya360-3.6.0.tar` & `ya360-3.6.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.860254 ya360-3.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.852254 ya360-3.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.852254 ya360-3.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-05 07:28:37.000000 ya360-3.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-05 07:28:37.000000 ya360-3.6.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-05 07:28:37.000000 ya360-3.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.852254 ya360-3.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-05 07:28:37.000000 ya360-3.6.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-05 07:28:37.000000 ya360-3.6.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-05 07:28:37.000000 ya360-3.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-05 07:28:37.000000 ya360-3.6.0/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.852254 ya360-3.6.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 07:28:37.000000 ya360-3.6.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-05 07:28:37.000000 ya360-3.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 07:28:37.000000 ya360-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 07:28:37.000000 ya360-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-05 07:28:42.860254 ya360-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-05 07:28:37.000000 ya360-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-05 07:28:37.000000 ya360-3.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-05 07:28:37.000000 ya360-3.6.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.852254 ya360-3.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.856254 ya360-3.6.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.856254 ya360-3.6.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    38353 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/_static/fig1.png
--rw-r--r--   0 runner    (1001) docker     (127)   127538 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/_static/fig2.png
--rw-r--r--   0 runner    (1001) docker     (127)    36447 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/_static/fig3.png
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/_static/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/befo.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/cmd.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/lic.rst
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/routing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-04-05 07:28:37.000000 ya360-3.6.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-05 07:28:37.000000 ya360-3.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 07:28:42.860254 ya360-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 07:28:37.000000 ya360-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.856254 ya360-3.6.0/ya360/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-05 07:28:42.000000 ya360-3.6.0/ya360/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/antispam.py
--rw-r--r--   0 runner    (1001) docker     (127)    31096 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/departments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/routing.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/tid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-05 07:28:37.000000 ya360-3.6.0/ya360/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:28:42.860254 ya360-3.6.0/ya360.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-05 07:28:42.000000 ya360-3.6.0/ya360.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-05 07:28:42.000000 ya360-3.6.0/ya360.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 07:28:42.000000 ya360-3.6.0/ya360.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 07:28:42.000000 ya360-3.6.0/ya360.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 07:28:42.000000 ya360-3.6.0/ya360.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 07:28:42.000000 ya360-3.6.0/ya360.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.218502 ya360-3.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.210502 ya360-3.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.210502 ya360-3.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-02 10:25:31.000000 ya360-3.6.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-02 10:25:31.000000 ya360-3.6.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-02 10:25:31.000000 ya360-3.6.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.210502 ya360-3.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-02 10:25:31.000000 ya360-3.6.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-02 10:25:31.000000 ya360-3.6.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-02 10:25:31.000000 ya360-3.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-02 10:25:31.000000 ya360-3.6.1/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.210502 ya360-3.6.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 10:25:31.000000 ya360-3.6.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-02 10:25:31.000000 ya360-3.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-02 10:25:31.000000 ya360-3.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 10:25:31.000000 ya360-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-02 10:25:36.218502 ya360-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-02 10:25:31.000000 ya360-3.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-02 10:25:31.000000 ya360-3.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 10:25:31.000000 ya360-3.6.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.210502 ya360-3.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.210502 ya360-3.6.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.214502 ya360-3.6.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    38353 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/_static/fig1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   127538 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/_static/fig2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36447 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/_static/fig3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/_static/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/befo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/cmd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/lic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/routing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-02 10:25:31.000000 ya360-3.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:25:36.218502 ya360-3.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-02 10:25:31.000000 ya360-3.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.214502 ya360-3.6.1/ya360/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 10:25:36.000000 ya360-3.6.1/ya360/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/antispam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31096 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/departments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/tid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.218502 ya360-3.6.1/ya360.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-02 10:25:36.000000 ya360-3.6.1/ya360.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-02 10:25:36.000000 ya360-3.6.1/ya360.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:25:36.000000 ya360-3.6.1/ya360.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 10:25:36.000000 ya360-3.6.1/ya360.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:25:36.000000 ya360-3.6.1/ya360.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 10:25:36.000000 ya360-3.6.1/ya360.egg-info/top_level.txt
```

### Comparing `ya360-3.6.0/.github/ISSUE_TEMPLATE/bug_report.md` & `ya360-3.6.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `ya360-3.6.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/.github/workflows/codeql-analysis.yml` & `ya360-3.6.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/.github/workflows/python-publish.yml` & `ya360-3.6.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/.gitignore` & `ya360-3.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/.readthedocs.yaml` & `ya360-3.6.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/CODE_OF_CONDUCT.md` & `ya360-3.6.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/LICENSE` & `ya360-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/PKG-INFO` & `ya360-3.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ya360
-Version: 3.6.0
+Version: 3.6.1
 Summary: Утилита командной строки для Yandex 360
 Author-email: Купцов Игорь <ya360@uh.net.ru>
 License: MIT
 Project-URL: Homepage, https://ya360.uh.net.ru
 Project-URL: Bug Tracker, https://github.com/imercury13/ya360/issues
 Project-URL: Documentation, https://ya360.readthedocs.io/
 Project-URL: Download, https://github.com/imercury13/ya360
```

### Comparing `ya360-3.6.0/README.md` & `ya360-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/README.rst` & `ya360-3.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/docs/Makefile` & `ya360-3.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/docs/make.bat` & `ya360-3.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/docs/source/_static/fig1.png` & `ya360-3.6.1/docs/source/_static/fig1.png`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/docs/source/_static/fig2.png` & `ya360-3.6.1/docs/source/_static/fig2.png`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/docs/source/_static/fig3.png` & `ya360-3.6.1/docs/source/_static/fig3.png`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/docs/source/befo.rst` & `ya360-3.6.1/docs/source/befo.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/docs/source/cmd.rst` & `ya360-3.6.1/docs/source/cmd.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/docs/source/conf.py` & `ya360-3.6.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/docs/source/index.rst` & `ya360-3.6.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/docs/source/lic.rst` & `ya360-3.6.1/docs/source/lic.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/docs/source/usage.rst` & `ya360-3.6.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/pyproject.toml` & `ya360-3.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/ya360/antispam.py` & `ya360-3.6.1/ya360/antispam.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/ya360/cmd.py` & `ya360-3.6.1/ya360/cmd.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/ya360/configure.py` & `ya360-3.6.1/ya360/configure.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/ya360/departments.py` & `ya360-3.6.1/ya360/departments.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/ya360/groups.py` & `ya360-3.6.1/ya360/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 		body.update({'type':'user', 'id':ret['id']})
 	ret = search_in_groups(args.member)
 	if 'id' in ret:
 		body.update({'type':'group', 'id':ret['id']})
 	ret = search_in_departments(args.member)
 	if 'id' in ret:
 		body.update({'type':'department', 'id':ret['id']})
-	check_request(groups.add_member_group(__token__, __orgid__, body, str(gid)))
+	check_request(groups.add_member_group(__token__, __orgid__, str(gid), body))
 	print('Добавлено')
 
 
 def delete_member_group(args):
 	"""Функция удаления участника из группы
 	
 	:param args: словарь аргументов командной строки
```

### Comparing `ya360-3.6.0/ya360/logs.py` & `ya360-3.6.1/ya360/logs.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/ya360/mail.py` & `ya360-3.6.1/ya360/mail.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/ya360/routing.py` & `ya360-3.6.1/ya360/routing.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/ya360/tid.py` & `ya360-3.6.1/ya360/tid.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/ya360/tools.py` & `ya360-3.6.1/ya360/tools.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/ya360/users.py` & `ya360-3.6.1/ya360/users.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/ya360/whois.py` & `ya360-3.6.1/ya360/whois.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.0/ya360.egg-info/PKG-INFO` & `ya360-3.6.1/ya360.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ya360
-Version: 3.6.0
+Version: 3.6.1
 Summary: Утилита командной строки для Yandex 360
 Author-email: Купцов Игорь <ya360@uh.net.ru>
 License: MIT
 Project-URL: Homepage, https://ya360.uh.net.ru
 Project-URL: Bug Tracker, https://github.com/imercury13/ya360/issues
 Project-URL: Documentation, https://ya360.readthedocs.io/
 Project-URL: Download, https://github.com/imercury13/ya360
```

### Comparing `ya360-3.6.0/ya360.egg-info/SOURCES.txt` & `ya360-3.6.1/ya360.egg-info/SOURCES.txt`

 * *Files identical despite different names*

