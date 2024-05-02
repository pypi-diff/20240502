# Comparing `tmp/comfy_cli-0.0.8.tar.gz` & `tmp/comfy_cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comfy_cli-0.0.8.tar", last modified: Thu May  2 01:04:59 2024, max compression
+gzip compressed data, was "comfy_cli-0.0.9.tar", last modified: Thu May  2 01:09:02 2024, max compression
```

## Comparing `comfy_cli-0.0.8.tar` & `comfy_cli-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:04:59.157584 comfy_cli-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    47626 2024-05-02 01:04:59.157584 comfy_cli-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:04:59.153584 comfy_cli-0.0.8/comfy_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11977 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/cmdline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:04:59.153584 comfy_cli-0.0.8/comfy_cli/command/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:04:59.157584 comfy_cli-0.0.8/comfy_cli/command/custom_nodes/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/command/custom_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/command/custom_nodes/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/command/install.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:04:59.157584 comfy_cli-0.0.8/comfy_cli/command/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/command/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/command/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/env_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/meta_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-02 01:04:52.000000 comfy_cli-0.0.8/comfy_cli/workspace_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:04:59.157584 comfy_cli-0.0.8/comfy_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    47626 2024-05-02 01:04:59.000000 comfy_cli-0.0.8/comfy_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-02 01:04:59.000000 comfy_cli-0.0.8/comfy_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:04:59.000000 comfy_cli-0.0.8/comfy_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-02 01:04:59.000000 comfy_cli-0.0.8/comfy_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 01:04:59.000000 comfy_cli-0.0.8/comfy_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 01:04:59.000000 comfy_cli-0.0.8/comfy_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-02 01:04:56.000000 comfy_cli-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 01:04:59.157584 comfy_cli-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:09:02.441331 comfy_cli-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    47626 2024-05-02 01:09:02.441331 comfy_cli-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:09:02.437331 comfy_cli-0.0.9/comfy_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11977 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/cmdline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:09:02.441331 comfy_cli-0.0.9/comfy_cli/command/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:09:02.441331 comfy_cli-0.0.9/comfy_cli/command/custom_nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/command/custom_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/command/custom_nodes/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/command/install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:09:02.441331 comfy_cli-0.0.9/comfy_cli/command/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/command/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/command/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/env_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/workspace_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:09:02.441331 comfy_cli-0.0.9/comfy_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    47626 2024-05-02 01:09:02.000000 comfy_cli-0.0.9/comfy_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-02 01:09:02.000000 comfy_cli-0.0.9/comfy_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:09:02.000000 comfy_cli-0.0.9/comfy_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-02 01:09:02.000000 comfy_cli-0.0.9/comfy_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 01:09:02.000000 comfy_cli-0.0.9/comfy_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 01:09:02.000000 comfy_cli-0.0.9/comfy_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-02 01:08:59.000000 comfy_cli-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 01:09:02.441331 comfy_cli-0.0.9/setup.cfg
```

### Comparing `comfy_cli-0.0.8/LICENSE` & `comfy_cli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.8/PKG-INFO` & `comfy_cli-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comfy-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: A CLI tool for installing and using ComfyUI.
 Maintainer-email: Yoland Yan <yoland@drip.art>, James Kwon <hongilkwon316@gmail.com>, Robin Huang <robin@drip.art>, "Dr.Lt.Data" <dr.lt.data@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `comfy_cli-0.0.8/README.md` & `comfy_cli-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.8/comfy_cli/cmdline.py` & `comfy_cli-0.0.9/comfy_cli/cmdline.py`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.8/comfy_cli/command/custom_nodes/command.py` & `comfy_cli-0.0.9/comfy_cli/command/custom_nodes/command.py`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.8/comfy_cli/command/install.py` & `comfy_cli-0.0.9/comfy_cli/command/install.py`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.8/comfy_cli/command/models/models.py` & `comfy_cli-0.0.9/comfy_cli/command/models/models.py`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.8/comfy_cli/config_manager.py` & `comfy_cli-0.0.9/comfy_cli/config_manager.py`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.8/comfy_cli/constants.py` & `comfy_cli-0.0.9/comfy_cli/constants.py`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.8/comfy_cli/env_checker.py` & `comfy_cli-0.0.9/comfy_cli/env_checker.py`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.8/comfy_cli/logging.py` & `comfy_cli-0.0.9/comfy_cli/logging.py`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.8/comfy_cli/meta_data.py` & `comfy_cli-0.0.9/comfy_cli/meta_data.py`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.8/comfy_cli/tracking.py` & `comfy_cli-0.0.9/comfy_cli/tracking.py`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.8/comfy_cli/ui.py` & `comfy_cli-0.0.9/comfy_cli/ui.py`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.8/comfy_cli/utils.py` & `comfy_cli-0.0.9/comfy_cli/utils.py`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.8/comfy_cli/workspace_manager.py` & `comfy_cli-0.0.9/comfy_cli/workspace_manager.py`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.8/comfy_cli.egg-info/PKG-INFO` & `comfy_cli-0.0.9/comfy_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comfy-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: A CLI tool for installing and using ComfyUI.
 Maintainer-email: Yoland Yan <yoland@drip.art>, James Kwon <hongilkwon316@gmail.com>, Robin Huang <robin@drip.art>, "Dr.Lt.Data" <dr.lt.data@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `comfy_cli-0.0.8/comfy_cli.egg-info/SOURCES.txt` & `comfy_cli-0.0.9/comfy_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.8/pyproject.toml` & `comfy_cli-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "comfy-cli"
 license = {file = "LICENSE"}
-version = "v0.0.8"
+version = "v0.0.9"
 requires-python = ">= 3.8"
 description = "A CLI tool for installing and using ComfyUI."
 readme = "README.md"
 keywords = ["comfyui", "stable diffusion"]
 
 maintainers = [
   {name = "Yoland Yan", email = "yoland@drip.art"},
```

