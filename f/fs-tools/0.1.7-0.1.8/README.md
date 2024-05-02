# Comparing `tmp/fs_tools-0.1.7.tar.gz` & `tmp/fs_tools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs_tools-0.1.7.tar", last modified: Thu Apr 25 07:26:33 2024, max compression
+gzip compressed data, was "fs_tools-0.1.8.tar", last modified: Thu Apr 25 07:28:13 2024, max compression
```

## Comparing `fs_tools-0.1.7.tar` & `fs_tools-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:26:33.774241 fs_tools-0.1.7/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      365 2024-04-25 07:26:33.764241 fs_tools-0.1.7/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-04-24 13:03:55.000000 fs_tools-0.1.7/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      548 2024-04-25 07:26:31.000000 fs_tools-0.1.7/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 07:26:33.774241 fs_tools-0.1.7/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:26:33.764241 fs_tools-0.1.7/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:26:33.764241 fs_tools-0.1.7/src/fs/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      166 2024-04-24 14:51:42.000000 fs_tools-0.1.7/src/fs/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      288 2024-04-24 14:52:16.000000 fs_tools-0.1.7/src/fs/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1152 2024-04-24 14:50:46.000000 fs_tools-0.1.7/src/fs/compression.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1971 2024-04-24 14:52:10.000000 fs_tools-0.1.7/src/fs/io.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      783 2024-04-24 14:21:15.000000 fs_tools-0.1.7/src/fs/moving.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      665 2024-04-25 07:26:10.000000 fs_tools-0.1.7/src/fs/paths.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:26:33.764241 fs_tools-0.1.7/src/fs_tools.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      365 2024-04-25 07:26:33.000000 fs_tools-0.1.7/src/fs_tools.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-04-25 07:26:33.000000 fs_tools-0.1.7/src/fs_tools.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 07:26:33.000000 fs_tools-0.1.7/src/fs_tools.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-25 07:26:33.000000 fs_tools-0.1.7/src/fs_tools.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-25 07:26:33.000000 fs_tools-0.1.7/src/fs_tools.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:28:13.514242 fs_tools-0.1.8/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      398 2024-04-25 07:28:13.514242 fs_tools-0.1.8/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-04-24 13:03:55.000000 fs_tools-0.1.8/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      569 2024-04-25 07:28:09.000000 fs_tools-0.1.8/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 07:28:13.514242 fs_tools-0.1.8/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:28:13.494242 fs_tools-0.1.8/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:28:13.504242 fs_tools-0.1.8/src/fs/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      166 2024-04-24 14:51:42.000000 fs_tools-0.1.8/src/fs/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      288 2024-04-24 14:52:16.000000 fs_tools-0.1.8/src/fs/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1152 2024-04-24 14:50:46.000000 fs_tools-0.1.8/src/fs/compression.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1971 2024-04-24 14:52:10.000000 fs_tools-0.1.8/src/fs/io.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      783 2024-04-24 14:21:15.000000 fs_tools-0.1.8/src/fs/moving.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      665 2024-04-25 07:26:10.000000 fs_tools-0.1.8/src/fs/paths.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:28:13.514242 fs_tools-0.1.8/src/fs_tools.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      398 2024-04-25 07:28:13.000000 fs_tools-0.1.8/src/fs_tools.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-04-25 07:28:13.000000 fs_tools-0.1.8/src/fs_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 07:28:13.000000 fs_tools-0.1.8/src/fs_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-04-25 07:28:13.000000 fs_tools-0.1.8/src/fs_tools.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-25 07:28:13.000000 fs_tools-0.1.8/src/fs_tools.egg-info/top_level.txt
```

### Comparing `fs_tools-0.1.7/pyproject.toml` & `fs_tools-0.1.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fs-tools"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple, exception-free filesystem tools"
 dependencies = [
-  "haskellian"
+  "haskellian", "typing-extensions"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/python-storage.git"
```

### Comparing `fs_tools-0.1.7/src/fs/compression.py` & `fs_tools-0.1.8/src/fs/compression.py`

 * *Files identical despite different names*

### Comparing `fs_tools-0.1.7/src/fs/io.py` & `fs_tools-0.1.8/src/fs/io.py`

 * *Files identical despite different names*

### Comparing `fs_tools-0.1.7/src/fs/moving.py` & `fs_tools-0.1.8/src/fs/moving.py`

 * *Files identical despite different names*

### Comparing `fs_tools-0.1.7/src/fs/paths.py` & `fs_tools-0.1.8/src/fs/paths.py`

 * *Files identical despite different names*

