# Comparing `tmp/peter_explains-0.0.11.tar.gz` & `tmp/peter-explains-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peter_explains-0.0.11.tar", last modified: Thu May  2 15:35:26 2024, max compression
+gzip compressed data, was "peter-explains-0.0.9.tar", last modified: Sun Mar 17 09:05:09 2024, max compression
```

## Comparing `peter_explains-0.0.11.tar` & `peter-explains-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:26.749394 peter_explains-0.0.11/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-02 15:35:16.000000 peter_explains-0.0.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-02 15:35:26.749394 peter_explains-0.0.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-02 15:35:16.000000 peter_explains-0.0.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:26.749394 peter_explains-0.0.11/peter_explains/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:16.000000 peter_explains-0.0.11/peter_explains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 15:35:16.000000 peter_explains-0.0.11/peter_explains/_name.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 15:35:16.000000 peter_explains-0.0.11/peter_explains/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-02 15:35:16.000000 peter_explains-0.0.11/peter_explains/api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-02 15:35:16.000000 peter_explains-0.0.11/peter_explains/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-02 15:35:16.000000 peter_explains-0.0.11/peter_explains/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-02 15:35:16.000000 peter_explains-0.0.11/peter_explains/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-02 15:35:16.000000 peter_explains-0.0.11/peter_explains/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-02 15:35:16.000000 peter_explains-0.0.11/peter_explains/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-02 15:35:16.000000 peter_explains-0.0.11/peter_explains/peter_ai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-02 15:35:16.000000 peter_explains-0.0.11/peter_explains/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-02 15:35:16.000000 peter_explains-0.0.11/peter_explains/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-02 15:35:16.000000 peter_explains-0.0.11/peter_explains/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:26.749394 peter_explains-0.0.11/peter_explains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-02 15:35:26.000000 peter_explains-0.0.11/peter_explains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-02 15:35:26.000000 peter_explains-0.0.11/peter_explains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:35:26.000000 peter_explains-0.0.11/peter_explains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-02 15:35:26.000000 peter_explains-0.0.11/peter_explains.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 15:35:26.000000 peter_explains-0.0.11/peter_explains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 15:35:26.000000 peter_explains-0.0.11/peter_explains.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:35:26.749394 peter_explains-0.0.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-02 15:35:16.000000 peter_explains-0.0.11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:26.749394 peter_explains-0.0.11/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:16.000000 peter_explains-0.0.11/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:09.224147 peter-explains-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-17 09:05:04.000000 peter-explains-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-03-17 09:05:09.224147 peter-explains-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-17 09:05:04.000000 peter-explains-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:09.224147 peter-explains-0.0.9/peter_explains/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:04.000000 peter-explains-0.0.9/peter_explains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-17 09:05:04.000000 peter-explains-0.0.9/peter_explains/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-17 09:05:04.000000 peter-explains-0.0.9/peter_explains/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-17 09:05:04.000000 peter-explains-0.0.9/peter_explains/peter_ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-03-17 09:05:04.000000 peter-explains-0.0.9/peter_explains/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:09.224147 peter-explains-0.0.9/peter_explains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-03-17 09:05:09.000000 peter-explains-0.0.9/peter_explains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-17 09:05:09.000000 peter-explains-0.0.9/peter_explains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 09:05:09.000000 peter-explains-0.0.9/peter_explains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-17 09:05:09.000000 peter-explains-0.0.9/peter_explains.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-17 09:05:09.000000 peter-explains-0.0.9/peter_explains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-17 09:05:09.000000 peter-explains-0.0.9/peter_explains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 09:05:09.224147 peter-explains-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-17 09:05:04.000000 peter-explains-0.0.9/setup.py
```

### Comparing `peter_explains-0.0.11/LICENSE` & `peter-explains-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `peter_explains-0.0.11/setup.py` & `peter-explains-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 from peter_explains import _version
-from peter_explains import _name
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
-    name=_name.__app_name__,
+    name="peter-explains",
     version=_version.__version__,
     description="Linux command explanations from Peter Griffin",
     author="Atick Faisal",
     author_email="atickfaisal@gmail.com",
     packages=find_packages(),
-    install_requires=[
-        "keyring",
-        "colorama",
-        "diskcache",
-        "json_repair",
-        "google-generativeai",
-    ],
+    install_requires=["colorama", "google-generativeai"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         "console_scripts": [
             "peter = peter_explains.main:peter",
         ],
     },
```

