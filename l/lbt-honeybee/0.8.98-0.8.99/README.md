# Comparing `tmp/lbt-honeybee-0.8.98.tar.gz` & `tmp/lbt-honeybee-0.8.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lbt-honeybee-0.8.98.tar", last modified: Wed Jan  3 21:19:27 2024, max compression
+gzip compressed data, was "dist/lbt-honeybee-0.8.99.tar", last modified: Wed Jan  3 23:03:43 2024, max compression
```

## Comparing `lbt-honeybee-0.8.98.tar` & `lbt-honeybee-0.8.99.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 21:19:27.000000 lbt-honeybee-0.8.98/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-03 21:18:13.000000 lbt-honeybee-0.8.98/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 21:19:27.000000 lbt-honeybee-0.8.98/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 21:19:27.000000 lbt-honeybee-0.8.98/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-01-03 21:18:13.000000 lbt-honeybee-0.8.98/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-01-03 21:18:13.000000 lbt-honeybee-0.8.98/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-03 21:18:13.000000 lbt-honeybee-0.8.98/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-01-03 21:18:13.000000 lbt-honeybee-0.8.98/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-03 21:18:13.000000 lbt-honeybee-0.8.98/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-01-03 21:18:13.000000 lbt-honeybee-0.8.98/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-01-03 21:18:13.000000 lbt-honeybee-0.8.98/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-03 21:18:13.000000 lbt-honeybee-0.8.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-01-03 21:19:27.000000 lbt-honeybee-0.8.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-01-03 21:18:13.000000 lbt-honeybee-0.8.98/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-01-03 21:18:13.000000 lbt-honeybee-0.8.98/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-03 21:18:13.000000 lbt-honeybee-0.8.98/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 21:19:27.000000 lbt-honeybee-0.8.98/lbt_honeybee/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-01-03 21:18:13.000000 lbt-honeybee-0.8.98/lbt_honeybee/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 21:19:27.000000 lbt-honeybee-0.8.98/lbt_honeybee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-01-03 21:19:27.000000 lbt-honeybee-0.8.98/lbt_honeybee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-01-03 21:19:27.000000 lbt-honeybee-0.8.98/lbt_honeybee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 21:19:27.000000 lbt-honeybee-0.8.98/lbt_honeybee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-03 21:19:27.000000 lbt-honeybee-0.8.98/lbt_honeybee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 21:19:27.000000 lbt-honeybee-0.8.98/lbt_honeybee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-03 21:18:13.000000 lbt-honeybee-0.8.98/pass_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-03 21:18:13.000000 lbt-honeybee-0.8.98/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-03 21:19:27.000000 lbt-honeybee-0.8.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-01-03 21:18:13.000000 lbt-honeybee-0.8.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 23:03:43.000000 lbt-honeybee-0.8.99/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-03 23:02:26.000000 lbt-honeybee-0.8.99/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 23:03:43.000000 lbt-honeybee-0.8.99/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 23:03:43.000000 lbt-honeybee-0.8.99/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-01-03 23:02:26.000000 lbt-honeybee-0.8.99/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-01-03 23:02:26.000000 lbt-honeybee-0.8.99/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-03 23:02:26.000000 lbt-honeybee-0.8.99/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-01-03 23:02:26.000000 lbt-honeybee-0.8.99/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-03 23:02:26.000000 lbt-honeybee-0.8.99/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-01-03 23:02:26.000000 lbt-honeybee-0.8.99/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-01-03 23:02:26.000000 lbt-honeybee-0.8.99/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-03 23:02:26.000000 lbt-honeybee-0.8.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-01-03 23:03:43.000000 lbt-honeybee-0.8.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-01-03 23:02:26.000000 lbt-honeybee-0.8.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-01-03 23:02:26.000000 lbt-honeybee-0.8.99/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-03 23:02:26.000000 lbt-honeybee-0.8.99/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 23:03:43.000000 lbt-honeybee-0.8.99/lbt_honeybee/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-01-03 23:02:26.000000 lbt-honeybee-0.8.99/lbt_honeybee/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 23:03:43.000000 lbt-honeybee-0.8.99/lbt_honeybee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-01-03 23:03:43.000000 lbt-honeybee-0.8.99/lbt_honeybee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-01-03 23:03:43.000000 lbt-honeybee-0.8.99/lbt_honeybee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 23:03:43.000000 lbt-honeybee-0.8.99/lbt_honeybee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-03 23:03:43.000000 lbt-honeybee-0.8.99/lbt_honeybee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 23:03:43.000000 lbt-honeybee-0.8.99/lbt_honeybee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-03 23:02:26.000000 lbt-honeybee-0.8.99/pass_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-03 23:02:26.000000 lbt-honeybee-0.8.99/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-03 23:03:43.000000 lbt-honeybee-0.8.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-01-03 23:02:26.000000 lbt-honeybee-0.8.99/setup.py
```

### Comparing `lbt-honeybee-0.8.98/.github/workflows/ci.yaml` & `lbt-honeybee-0.8.99/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `lbt-honeybee-0.8.98/.github/workflows/dependency-release.yaml` & `lbt-honeybee-0.8.99/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `lbt-honeybee-0.8.98/Dockerfile` & `lbt-honeybee-0.8.99/Dockerfile`

 * *Files identical despite different names*

### Comparing `lbt-honeybee-0.8.98/LICENSE` & `lbt-honeybee-0.8.99/LICENSE`

 * *Files identical despite different names*

### Comparing `lbt-honeybee-0.8.98/PKG-INFO` & `lbt-honeybee-0.8.99/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbt-honeybee
-Version: 0.8.98
+Version: 0.8.99
 Summary: Installs a collection of all Honeybee core and extension libraries.
 Home-page: https://github.com/ladybug-tools/lbt-honeybee
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `lbt-honeybee-0.8.98/README.md` & `lbt-honeybee-0.8.99/README.md`

 * *Files identical despite different names*

### Comparing `lbt-honeybee-0.8.98/deploy.sh` & `lbt-honeybee-0.8.99/deploy.sh`

 * *Files identical despite different names*

### Comparing `lbt-honeybee-0.8.98/lbt_honeybee.egg-info/PKG-INFO` & `lbt-honeybee-0.8.99/lbt_honeybee.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbt-honeybee
-Version: 0.8.98
+Version: 0.8.99
 Summary: Installs a collection of all Honeybee core and extension libraries.
 Home-page: https://github.com/ladybug-tools/lbt-honeybee
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `lbt-honeybee-0.8.98/setup.py` & `lbt-honeybee-0.8.99/setup.py`

 * *Files identical despite different names*

