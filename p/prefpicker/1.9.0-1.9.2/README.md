# Comparing `tmp/prefpicker-1.9.0.tar.gz` & `tmp/prefpicker-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefpicker-1.9.0.tar", last modified: Mon Mar 27 17:27:59 2023, max compression
+gzip compressed data, was "prefpicker-1.9.2.tar", last modified: Thu Apr 27 16:41:37 2023, max compression
```

## Comparing `prefpicker-1.9.0.tar` & `prefpicker-1.9.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-03-27 17:27:59.319764 prefpicker-1.9.0/
--rw-r--r--   0 worker    (1000) worker    (1000)       55 2023-03-27 17:27:48.000000 prefpicker-1.9.0/.codecov.yml
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-03-27 17:27:59.311763 prefpicker-1.9.0/.github/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-03-27 17:27:59.315763 prefpicker-1.9.0/.github/workflows/
--rw-r--r--   0 worker    (1000) worker    (1000)      563 2023-03-27 17:27:48.000000 prefpicker-1.9.0/.github/workflows/prefmonitor.yml
--rw-r--r--   0 worker    (1000) worker    (1000)     1073 2023-03-27 17:27:48.000000 prefpicker-1.9.0/.gitignore
--rw-r--r--   0 worker    (1000) worker    (1000)     2248 2023-03-27 17:27:48.000000 prefpicker-1.9.0/.pre-commit-config.yaml
--rw-r--r--   0 worker    (1000) worker    (1000)     3914 2023-03-27 17:27:48.000000 prefpicker-1.9.0/.taskcluster.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      689 2023-03-27 17:27:48.000000 prefpicker-1.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 worker    (1000) worker    (1000)    16725 2023-03-27 17:27:48.000000 prefpicker-1.9.0/LICENSE
--rw-r--r--   0 worker    (1000) worker    (1000)       39 2023-03-27 17:27:48.000000 prefpicker-1.9.0/MANIFEST.in
--rw-r--r--   0 worker    (1000) worker    (1000)     5036 2023-03-27 17:27:59.319764 prefpicker-1.9.0/PKG-INFO
--rw-r--r--   0 worker    (1000) worker    (1000)     4401 2023-03-27 17:27:57.000000 prefpicker-1.9.0/README.md
--rw-r--r--   0 worker    (1000) worker    (1000)      857 2023-03-27 17:27:48.000000 prefpicker-1.9.0/pyproject.toml
--rw-r--r--   0 worker    (1000) worker    (1000)     1131 2023-03-27 17:27:59.319764 prefpicker-1.9.0/setup.cfg
--rwxr-xr-x   0 worker    (1000) worker    (1000)      370 2023-03-27 17:27:48.000000 prefpicker-1.9.0/setup.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-03-27 17:27:59.311763 prefpicker-1.9.0/src/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-03-27 17:27:59.315763 prefpicker-1.9.0/src/prefpicker/
--rw-r--r--   0 worker    (1000) worker    (1000)      348 2023-03-27 17:27:48.000000 prefpicker-1.9.0/src/prefpicker/__init__.py
--rw-r--r--   0 worker    (1000) worker    (1000)      282 2023-03-27 17:27:48.000000 prefpicker-1.9.0/src/prefpicker/__main__.py
--rw-r--r--   0 worker    (1000) worker    (1000)     3359 2023-03-27 17:27:48.000000 prefpicker-1.9.0/src/prefpicker/main.py
--rw-r--r--   0 worker    (1000) worker    (1000)     9134 2023-03-27 17:27:48.000000 prefpicker-1.9.0/src/prefpicker/prefpicker.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-03-27 17:27:59.319764 prefpicker-1.9.0/src/prefpicker/templates/
--rw-r--r--   0 worker    (1000) worker    (1000)    19341 2023-03-27 17:27:48.000000 prefpicker-1.9.0/src/prefpicker/templates/browser-fuzzing.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      898 2023-03-27 17:27:48.000000 prefpicker-1.9.0/src/prefpicker/templates/schema.json
--rw-r--r--   0 worker    (1000) worker    (1000)     2644 2023-03-27 17:27:48.000000 prefpicker-1.9.0/src/prefpicker/test_main.py
--rw-r--r--   0 worker    (1000) worker    (1000)     8807 2023-03-27 17:27:48.000000 prefpicker-1.9.0/src/prefpicker/test_prefpicker.py
--rw-r--r--   0 worker    (1000) worker    (1000)     1496 2023-03-27 17:27:48.000000 prefpicker-1.9.0/src/prefpicker/test_templates.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-03-27 17:27:59.319764 prefpicker-1.9.0/src/prefpicker.egg-info/
--rw-r--r--   0 worker    (1000) worker    (1000)     5036 2023-03-27 17:27:59.000000 prefpicker-1.9.0/src/prefpicker.egg-info/PKG-INFO
--rw-r--r--   0 worker    (1000) worker    (1000)      739 2023-03-27 17:27:59.000000 prefpicker-1.9.0/src/prefpicker.egg-info/SOURCES.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-03-27 17:27:59.000000 prefpicker-1.9.0/src/prefpicker.egg-info/dependency_links.txt
--rw-r--r--   0 worker    (1000) worker    (1000)       52 2023-03-27 17:27:59.000000 prefpicker-1.9.0/src/prefpicker.egg-info/entry_points.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-03-27 17:27:59.000000 prefpicker-1.9.0/src/prefpicker.egg-info/not-zip-safe
--rw-r--r--   0 worker    (1000) worker    (1000)       29 2023-03-27 17:27:59.000000 prefpicker-1.9.0/src/prefpicker.egg-info/requires.txt
--rw-r--r--   0 worker    (1000) worker    (1000)       11 2023-03-27 17:27:59.000000 prefpicker-1.9.0/src/prefpicker.egg-info/top_level.txt
--rw-r--r--   0 worker    (1000) worker    (1000)     1118 2023-03-27 17:27:48.000000 prefpicker-1.9.0/tox.ini
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-04-27 16:41:37.462994 prefpicker-1.9.2/
+-rw-r--r--   0 worker    (1000) worker    (1000)       55 2023-04-27 16:41:24.000000 prefpicker-1.9.2/.codecov.yml
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-04-27 16:41:37.458994 prefpicker-1.9.2/.github/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-04-27 16:41:37.462994 prefpicker-1.9.2/.github/workflows/
+-rw-r--r--   0 worker    (1000) worker    (1000)      563 2023-04-27 16:41:24.000000 prefpicker-1.9.2/.github/workflows/prefmonitor.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)     1073 2023-04-27 16:41:24.000000 prefpicker-1.9.2/.gitignore
+-rw-r--r--   0 worker    (1000) worker    (1000)     2248 2023-04-27 16:41:24.000000 prefpicker-1.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 worker    (1000) worker    (1000)     3914 2023-04-27 16:41:24.000000 prefpicker-1.9.2/.taskcluster.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      689 2023-04-27 16:41:24.000000 prefpicker-1.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 worker    (1000) worker    (1000)    16725 2023-04-27 16:41:24.000000 prefpicker-1.9.2/LICENSE
+-rw-r--r--   0 worker    (1000) worker    (1000)       39 2023-04-27 16:41:24.000000 prefpicker-1.9.2/MANIFEST.in
+-rw-r--r--   0 worker    (1000) worker    (1000)     5036 2023-04-27 16:41:37.462994 prefpicker-1.9.2/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)     4401 2023-04-27 16:41:35.000000 prefpicker-1.9.2/README.md
+-rw-r--r--   0 worker    (1000) worker    (1000)      857 2023-04-27 16:41:24.000000 prefpicker-1.9.2/pyproject.toml
+-rw-r--r--   0 worker    (1000) worker    (1000)     1131 2023-04-27 16:41:37.466995 prefpicker-1.9.2/setup.cfg
+-rwxr-xr-x   0 worker    (1000) worker    (1000)      370 2023-04-27 16:41:24.000000 prefpicker-1.9.2/setup.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-04-27 16:41:37.458994 prefpicker-1.9.2/src/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-04-27 16:41:37.462994 prefpicker-1.9.2/src/prefpicker/
+-rw-r--r--   0 worker    (1000) worker    (1000)      348 2023-04-27 16:41:24.000000 prefpicker-1.9.2/src/prefpicker/__init__.py
+-rw-r--r--   0 worker    (1000) worker    (1000)      282 2023-04-27 16:41:24.000000 prefpicker-1.9.2/src/prefpicker/__main__.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     3359 2023-04-27 16:41:24.000000 prefpicker-1.9.2/src/prefpicker/main.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     9134 2023-04-27 16:41:24.000000 prefpicker-1.9.2/src/prefpicker/prefpicker.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-04-27 16:41:37.462994 prefpicker-1.9.2/src/prefpicker/templates/
+-rw-r--r--   0 worker    (1000) worker    (1000)    19328 2023-04-27 16:41:24.000000 prefpicker-1.9.2/src/prefpicker/templates/browser-fuzzing.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      898 2023-04-27 16:41:24.000000 prefpicker-1.9.2/src/prefpicker/templates/schema.json
+-rw-r--r--   0 worker    (1000) worker    (1000)     2644 2023-04-27 16:41:24.000000 prefpicker-1.9.2/src/prefpicker/test_main.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     8807 2023-04-27 16:41:24.000000 prefpicker-1.9.2/src/prefpicker/test_prefpicker.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     1496 2023-04-27 16:41:24.000000 prefpicker-1.9.2/src/prefpicker/test_templates.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-04-27 16:41:37.462994 prefpicker-1.9.2/src/prefpicker.egg-info/
+-rw-r--r--   0 worker    (1000) worker    (1000)     5036 2023-04-27 16:41:37.000000 prefpicker-1.9.2/src/prefpicker.egg-info/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)      739 2023-04-27 16:41:37.000000 prefpicker-1.9.2/src/prefpicker.egg-info/SOURCES.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-04-27 16:41:37.000000 prefpicker-1.9.2/src/prefpicker.egg-info/dependency_links.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)       52 2023-04-27 16:41:37.000000 prefpicker-1.9.2/src/prefpicker.egg-info/entry_points.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-04-27 16:41:37.000000 prefpicker-1.9.2/src/prefpicker.egg-info/not-zip-safe
+-rw-r--r--   0 worker    (1000) worker    (1000)       29 2023-04-27 16:41:37.000000 prefpicker-1.9.2/src/prefpicker.egg-info/requires.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)       11 2023-04-27 16:41:37.000000 prefpicker-1.9.2/src/prefpicker.egg-info/top_level.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)     1140 2023-04-27 16:41:24.000000 prefpicker-1.9.2/tox.ini
```

### Comparing `prefpicker-1.9.0/.github/workflows/prefmonitor.yml` & `prefpicker-1.9.2/.github/workflows/prefmonitor.yml`

 * *Files identical despite different names*

### Comparing `prefpicker-1.9.0/.gitignore` & `prefpicker-1.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `prefpicker-1.9.0/.pre-commit-config.yaml` & `prefpicker-1.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `prefpicker-1.9.0/.taskcluster.yml` & `prefpicker-1.9.2/.taskcluster.yml`

 * *Files identical despite different names*

### Comparing `prefpicker-1.9.0/CODE_OF_CONDUCT.md` & `prefpicker-1.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `prefpicker-1.9.0/LICENSE` & `prefpicker-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prefpicker-1.9.0/PKG-INFO` & `prefpicker-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefpicker
-Version: 1.9.0
+Version: 1.9.2
 Summary: PrefPicker - Manage & generate prefs.js files
 Home-page: https://github.com/MozillaSecurity/prefpicker
 Author: Tyson Smith
 Author-email: twsmith@mozilla.com
 Maintainer: Mozilla Fuzzing Team
 Maintainer-email: fuzzing@mozilla.com
 License: MPL 2.0
```

### Comparing `prefpicker-1.9.0/README.md` & `prefpicker-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `prefpicker-1.9.0/pyproject.toml` & `prefpicker-1.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefpicker-1.9.0/setup.cfg` & `prefpicker-1.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefpicker-1.9.0/src/prefpicker/main.py` & `prefpicker-1.9.2/src/prefpicker/main.py`

 * *Files identical despite different names*

### Comparing `prefpicker-1.9.0/src/prefpicker/prefpicker.py` & `prefpicker-1.9.2/src/prefpicker/prefpicker.py`

 * *Files identical despite different names*

### Comparing `prefpicker-1.9.0/src/prefpicker/templates/browser-fuzzing.yml` & `prefpicker-1.9.2/src/prefpicker/templates/browser-fuzzing.yml`

 * *Files 0% similar despite different names*

```diff
@@ -610,15 +610,14 @@
       jit:
       - 2
   javascript.options.ion.offthread_compilation:
     variants:
       default:
       - null
       jit:
-      - true
       - false
   javascript.options.ion.threshold:
     variants:
       default:
       - null
       jit:
       - 10
```

### Comparing `prefpicker-1.9.0/src/prefpicker/templates/schema.json` & `prefpicker-1.9.2/src/prefpicker/templates/schema.json`

 * *Files identical despite different names*

### Comparing `prefpicker-1.9.0/src/prefpicker/test_main.py` & `prefpicker-1.9.2/src/prefpicker/test_main.py`

 * *Files identical despite different names*

### Comparing `prefpicker-1.9.0/src/prefpicker/test_prefpicker.py` & `prefpicker-1.9.2/src/prefpicker/test_prefpicker.py`

 * *Files identical despite different names*

### Comparing `prefpicker-1.9.0/src/prefpicker/test_templates.py` & `prefpicker-1.9.2/src/prefpicker/test_templates.py`

 * *Files identical despite different names*

### Comparing `prefpicker-1.9.0/src/prefpicker.egg-info/PKG-INFO` & `prefpicker-1.9.2/src/prefpicker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefpicker
-Version: 1.9.0
+Version: 1.9.2
 Summary: PrefPicker - Manage & generate prefs.js files
 Home-page: https://github.com/MozillaSecurity/prefpicker
 Author: Tyson Smith
 Author-email: twsmith@mozilla.com
 Maintainer: Mozilla Fuzzing Team
 Maintainer-email: fuzzing@mozilla.com
 License: MPL 2.0
```

### Comparing `prefpicker-1.9.0/src/prefpicker.egg-info/SOURCES.txt` & `prefpicker-1.9.2/src/prefpicker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefpicker-1.9.0/tox.ini` & `prefpicker-1.9.2/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,18 @@
     VCS_*
 usedevelop = true
 
 [testenv:codecov]
 commands =
     codecov
 deps =
-    codecov
     coverage[toml]
 skip_install = true
+allowlist_externals =
+    codecov
 
 [testenv:lint]
 commands =
     pre-commit run -a {posargs}
 deps =
     pre-commit
 skip_install = true
```

