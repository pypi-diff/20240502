# Comparing `tmp/aise_toolkit_demo-0.2.tar.gz` & `tmp/aise_toolkit_demo-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aise_toolkit_demo-0.2.tar", last modified: Thu May  2 15:00:39 2024, max compression
+gzip compressed data, was "aise_toolkit_demo-0.3.tar", last modified: Thu May  2 16:09:32 2024, max compression
```

## Comparing `aise_toolkit_demo-0.2.tar` & `aise_toolkit_demo-0.3.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:00:39.023937 aise_toolkit_demo-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 15:00:32.000000 aise_toolkit_demo-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-02 15:00:39.023937 aise_toolkit_demo-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-02 15:00:32.000000 aise_toolkit_demo-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:00:39.019936 aise_toolkit_demo-0.2/aise_toolkit_demo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:00:32.000000 aise_toolkit_demo-0.2/aise_toolkit_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 15:00:32.000000 aise_toolkit_demo-0.2/aise_toolkit_demo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-02 15:00:32.000000 aise_toolkit_demo-0.2/aise_toolkit_demo/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:00:39.023937 aise_toolkit_demo-0.2/aise_toolkit_demo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-02 15:00:39.000000 aise_toolkit_demo-0.2/aise_toolkit_demo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-02 15:00:39.000000 aise_toolkit_demo-0.2/aise_toolkit_demo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:00:39.000000 aise_toolkit_demo-0.2/aise_toolkit_demo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 15:00:39.000000 aise_toolkit_demo-0.2/aise_toolkit_demo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 15:00:39.000000 aise_toolkit_demo-0.2/aise_toolkit_demo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 15:00:39.000000 aise_toolkit_demo-0.2/aise_toolkit_demo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-02 15:00:32.000000 aise_toolkit_demo-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:00:39.023937 aise_toolkit_demo-0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:00:39.023937 aise_toolkit_demo-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-02 15:00:32.000000 aise_toolkit_demo-0.2/tests/test_aise_toolkit_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:09:32.326436 aise_toolkit_demo-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 16:09:23.000000 aise_toolkit_demo-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-02 16:09:32.326436 aise_toolkit_demo-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-02 16:09:23.000000 aise_toolkit_demo-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:09:32.322436 aise_toolkit_demo-0.3/aise_toolkit_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:09:23.000000 aise_toolkit_demo-0.3/aise_toolkit_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 16:09:23.000000 aise_toolkit_demo-0.3/aise_toolkit_demo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:09:32.322436 aise_toolkit_demo-0.3/aise_toolkit_demo/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 16:09:23.000000 aise_toolkit_demo-0.3/aise_toolkit_demo/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-02 16:09:23.000000 aise_toolkit_demo-0.3/aise_toolkit_demo/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:09:32.326436 aise_toolkit_demo-0.3/aise_toolkit_demo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-02 16:09:32.000000 aise_toolkit_demo-0.3/aise_toolkit_demo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-02 16:09:32.000000 aise_toolkit_demo-0.3/aise_toolkit_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:09:32.000000 aise_toolkit_demo-0.3/aise_toolkit_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 16:09:32.000000 aise_toolkit_demo-0.3/aise_toolkit_demo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 16:09:32.000000 aise_toolkit_demo-0.3/aise_toolkit_demo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 16:09:32.000000 aise_toolkit_demo-0.3/aise_toolkit_demo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-02 16:09:23.000000 aise_toolkit_demo-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:09:32.326436 aise_toolkit_demo-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:09:32.322436 aise_toolkit_demo-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-02 16:09:23.000000 aise_toolkit_demo-0.3/tests/test_aise_toolkit_demo.py
```

### Comparing `aise_toolkit_demo-0.2/LICENSE` & `aise_toolkit_demo-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aise_toolkit_demo-0.2/PKG-INFO` & `aise_toolkit_demo-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aise-toolkit-demo
-Version: 0.2
+Version: 0.3
 Summary: A set of tools to assist developer to use AI
 Author: Lei Xu
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/ups216/aise-toolkit-demo
 Project-URL: Changelog, https://github.com/ups216/aise-toolkit-demo/releases
 Project-URL: Issues, https://github.com/ups216/aise-toolkit-demo/issues
 Project-URL: CI, https://github.com/ups216/aise-toolkit-demo/actions
```

### Comparing `aise_toolkit_demo-0.2/README.md` & `aise_toolkit_demo-0.3/README.md`

 * *Files identical despite different names*

### Comparing `aise_toolkit_demo-0.2/aise_toolkit_demo.egg-info/PKG-INFO` & `aise_toolkit_demo-0.3/aise_toolkit_demo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aise-toolkit-demo
-Version: 0.2
+Version: 0.3
 Summary: A set of tools to assist developer to use AI
 Author: Lei Xu
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/ups216/aise-toolkit-demo
 Project-URL: Changelog, https://github.com/ups216/aise-toolkit-demo/releases
 Project-URL: Issues, https://github.com/ups216/aise-toolkit-demo/issues
 Project-URL: CI, https://github.com/ups216/aise-toolkit-demo/actions
```

### Comparing `aise_toolkit_demo-0.2/pyproject.toml` & `aise_toolkit_demo-0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aise-toolkit-demo"
-version = "0.2"
+version = "0.3"
 description = "A set of tools to assist developer to use AI"
 readme = "README.md"
 authors = [{name = "Lei Xu"}]
 license = {text = "Apache-2.0"}
 requires-python = ">=3.8"
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
```

### Comparing `aise_toolkit_demo-0.2/tests/test_aise_toolkit_demo.py` & `aise_toolkit_demo-0.3/tests/test_aise_toolkit_demo.py`

 * *Files identical despite different names*

