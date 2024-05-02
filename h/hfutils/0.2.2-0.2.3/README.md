# Comparing `tmp/hfutils-0.2.2.tar.gz` & `tmp/hfutils-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfutils-0.2.2.tar", last modified: Sun Apr 21 10:44:53 2024, max compression
+gzip compressed data, was "hfutils-0.2.3.tar", last modified: Thu May  2 13:31:05 2024, max compression
```

## Comparing `hfutils-0.2.2.tar` & `hfutils-0.2.3.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:53.574517 hfutils-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-21 10:44:35.000000 hfutils-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-21 10:44:35.000000 hfutils-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-04-21 10:44:53.574517 hfutils-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-04-21 10:44:35.000000 hfutils-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:53.566516 hfutils-0.2.2/hfutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:53.566516 hfutils-0.2.2/hfutils/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/archive/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/archive/rar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/archive/sevenz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/archive/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/archive/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:53.566516 hfutils-0.2.2/hfutils/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:53.570517 hfutils-0.2.2/hfutils/entry/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/entry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/entry/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/entry/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/entry/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/entry/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/entry/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/entry/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:53.570517 hfutils-0.2.2/hfutils/index/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/index/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/index/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/index/make.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/index/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:53.570517 hfutils-0.2.2/hfutils/operate/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/operate/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/operate/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/operate/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/operate/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:53.570517 hfutils-0.2.2/hfutils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/utils/temp.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/utils/tqdm_.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-21 10:44:35.000000 hfutils-0.2.2/hfutils/utils/walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:53.570517 hfutils-0.2.2/hfutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-04-21 10:44:53.000000 hfutils-0.2.2/hfutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-21 10:44:53.000000 hfutils-0.2.2/hfutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 10:44:53.000000 hfutils-0.2.2/hfutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-21 10:44:53.000000 hfutils-0.2.2/hfutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-21 10:44:53.000000 hfutils-0.2.2/hfutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 10:44:53.000000 hfutils-0.2.2/hfutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-21 10:44:35.000000 hfutils-0.2.2/requirements-7z.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-21 10:44:35.000000 hfutils-0.2.2/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-21 10:44:35.000000 hfutils-0.2.2/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 10:44:35.000000 hfutils-0.2.2/requirements-rar.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-21 10:44:35.000000 hfutils-0.2.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 10:44:35.000000 hfutils-0.2.2/requirements-transfer.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-21 10:44:35.000000 hfutils-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 10:44:53.574517 hfutils-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-21 10:44:35.000000 hfutils-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.633952 hfutils-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 13:30:45.000000 hfutils-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-02 13:30:45.000000 hfutils-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-05-02 13:31:05.633952 hfutils-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-02 13:30:45.000000 hfutils-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.625952 hfutils-0.2.3/hfutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.625952 hfutils-0.2.3/hfutils/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/archive/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/archive/rar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/archive/sevenz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/archive/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/archive/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.625952 hfutils-0.2.3/hfutils/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.625952 hfutils-0.2.3/hfutils/entry/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/entry/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/entry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/entry/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/entry/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/entry/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/entry/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/entry/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.625952 hfutils-0.2.3/hfutils/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/index/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/index/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/index/make.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/index/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.629952 hfutils-0.2.3/hfutils/operate/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/operate/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/operate/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/operate/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/operate/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.629952 hfutils-0.2.3/hfutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/utils/temp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/utils/tqdm_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/utils/walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.629952 hfutils-0.2.3/hfutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-05-02 13:31:05.000000 hfutils-0.2.3/hfutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-02 13:31:05.000000 hfutils-0.2.3/hfutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:31:05.000000 hfutils-0.2.3/hfutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 13:31:05.000000 hfutils-0.2.3/hfutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-02 13:31:05.000000 hfutils-0.2.3/hfutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 13:31:05.000000 hfutils-0.2.3/hfutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 13:30:45.000000 hfutils-0.2.3/requirements-7z.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 13:30:45.000000 hfutils-0.2.3/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-02 13:30:45.000000 hfutils-0.2.3/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:30:45.000000 hfutils-0.2.3/requirements-rar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-02 13:30:45.000000 hfutils-0.2.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 13:30:45.000000 hfutils-0.2.3/requirements-transfer.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 13:30:45.000000 hfutils-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:31:05.633952 hfutils-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-02 13:30:45.000000 hfutils-0.2.3/setup.py
```

### Comparing `hfutils-0.2.2/LICENSE` & `hfutils-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/PKG-INFO` & `hfutils-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.2.2
+Version: 0.2.3
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hfutils-0.2.2/README.md` & `hfutils-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/archive/__init__.py` & `hfutils-0.2.3/hfutils/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/archive/base.py` & `hfutils-0.2.3/hfutils/archive/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/archive/rar.py` & `hfutils-0.2.3/hfutils/archive/rar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/archive/sevenz.py` & `hfutils-0.2.3/hfutils/archive/sevenz.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/archive/tar.py` & `hfutils-0.2.3/hfutils/archive/tar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/archive/zip.py` & `hfutils-0.2.3/hfutils/archive/zip.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/entry/base.py` & `hfutils-0.2.3/hfutils/entry/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/entry/dispatch.py` & `hfutils-0.2.3/hfutils/entry/dispatch.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/entry/download.py` & `hfutils-0.2.3/hfutils/entry/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/entry/ls.py` & `hfutils-0.2.3/hfutils/entry/ls.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/entry/upload.py` & `hfutils-0.2.3/hfutils/entry/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/index/fetch.py` & `hfutils-0.2.3/hfutils/index/fetch.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/index/hash.py` & `hfutils-0.2.3/hfutils/index/hash.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/index/make.py` & `hfutils-0.2.3/hfutils/index/make.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/index/validate.py` & `hfutils-0.2.3/hfutils/index/validate.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/operate/base.py` & `hfutils-0.2.3/hfutils/operate/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/operate/download.py` & `hfutils-0.2.3/hfutils/operate/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/operate/upload.py` & `hfutils-0.2.3/hfutils/operate/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/operate/validate.py` & `hfutils-0.2.3/hfutils/operate/validate.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/utils/binary.py` & `hfutils-0.2.3/hfutils/utils/binary.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/utils/download.py` & `hfutils-0.2.3/hfutils/utils/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/utils/temp.py` & `hfutils-0.2.3/hfutils/utils/temp.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/utils/tqdm_.py` & `hfutils-0.2.3/hfutils/utils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils/utils/walk.py` & `hfutils-0.2.3/hfutils/utils/walk.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/hfutils.egg-info/PKG-INFO` & `hfutils-0.2.3/hfutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.2.2
+Version: 0.2.3
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hfutils-0.2.2/hfutils.egg-info/SOURCES.txt` & `hfutils-0.2.3/hfutils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 hfutils/entry/__init__.py
 hfutils/entry/base.py
 hfutils/entry/cli.py
 hfutils/entry/dispatch.py
 hfutils/entry/download.py
 hfutils/entry/ls.py
 hfutils/entry/upload.py
+hfutils/entry/whoami.py
 hfutils/index/__init__.py
 hfutils/index/fetch.py
 hfutils/index/hash.py
 hfutils/index/make.py
 hfutils/index/validate.py
 hfutils/operate/__init__.py
 hfutils/operate/base.py
```

### Comparing `hfutils-0.2.2/hfutils.egg-info/requires.txt` & `hfutils-0.2.3/hfutils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.2/setup.py` & `hfutils-0.2.3/setup.py`

 * *Files identical despite different names*

