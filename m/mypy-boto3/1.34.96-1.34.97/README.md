# Comparing `tmp/mypy_boto3-1.34.96.tar.gz` & `tmp/mypy_boto3-1.34.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3-1.34.96.tar", last modified: Wed May  1 19:21:12 2024, max compression
+gzip compressed data, was "mypy_boto3-1.34.97.tar", last modified: Thu May  2 19:33:12 2024, max compression
```

## Comparing `mypy_boto3-1.34.96.tar` & `mypy_boto3-1.34.97.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:12.904299 mypy_boto3-1.34.96/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 19:19:45.000000 mypy_boto3-1.34.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-01 19:21:12.904299 mypy_boto3-1.34.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-01 19:19:45.000000 mypy_boto3-1.34.96/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:12.904299 mypy_boto3-1.34.96/mypy_boto3/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 19:19:45.000000 mypy_boto3-1.34.96/mypy_boto3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-01 19:19:45.000000 mypy_boto3-1.34.96/mypy_boto3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-01 19:19:47.000000 mypy_boto3-1.34.96/mypy_boto3/boto3_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-01 19:19:45.000000 mypy_boto3-1.34.96/mypy_boto3/boto3_init_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-01 19:19:45.000000 mypy_boto3-1.34.96/mypy_boto3/boto3_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-01 19:19:45.000000 mypy_boto3-1.34.96/mypy_boto3/boto3_session_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-01 19:19:45.000000 mypy_boto3-1.34.96/mypy_boto3/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-05-01 19:19:47.000000 mypy_boto3-1.34.96/mypy_boto3/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:19:45.000000 mypy_boto3-1.34.96/mypy_boto3/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   116366 2024-05-01 19:19:47.000000 mypy_boto3-1.34.96/mypy_boto3/submodules.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 19:19:45.000000 mypy_boto3-1.34.96/mypy_boto3/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:12.904299 mypy_boto3-1.34.96/mypy_boto3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-01 19:21:12.000000 mypy_boto3-1.34.96/mypy_boto3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-01 19:21:12.000000 mypy_boto3-1.34.96/mypy_boto3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:12.000000 mypy_boto3-1.34.96/mypy_boto3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:12.000000 mypy_boto3-1.34.96/mypy_boto3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-01 19:21:12.000000 mypy_boto3-1.34.96/mypy_boto3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 19:21:12.000000 mypy_boto3-1.34.96/mypy_boto3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:21:12.904299 mypy_boto3-1.34.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-01 19:19:45.000000 mypy_boto3-1.34.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:33:12.058103 mypy_boto3-1.34.97/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 19:31:52.000000 mypy_boto3-1.34.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-02 19:33:12.058103 mypy_boto3-1.34.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-02 19:31:52.000000 mypy_boto3-1.34.97/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:33:12.054103 mypy_boto3-1.34.97/mypy_boto3/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-02 19:31:52.000000 mypy_boto3-1.34.97/mypy_boto3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 19:31:52.000000 mypy_boto3-1.34.97/mypy_boto3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-02 19:31:54.000000 mypy_boto3-1.34.97/mypy_boto3/boto3_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-02 19:31:52.000000 mypy_boto3-1.34.97/mypy_boto3/boto3_init_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-02 19:31:52.000000 mypy_boto3-1.34.97/mypy_boto3/boto3_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-02 19:31:52.000000 mypy_boto3-1.34.97/mypy_boto3/boto3_session_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-02 19:31:52.000000 mypy_boto3-1.34.97/mypy_boto3/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-05-02 19:31:54.000000 mypy_boto3-1.34.97/mypy_boto3/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:31:52.000000 mypy_boto3-1.34.97/mypy_boto3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   116366 2024-05-02 19:31:54.000000 mypy_boto3-1.34.97/mypy_boto3/submodules.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 19:31:52.000000 mypy_boto3-1.34.97/mypy_boto3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:33:12.058103 mypy_boto3-1.34.97/mypy_boto3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-02 19:33:12.000000 mypy_boto3-1.34.97/mypy_boto3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-02 19:33:12.000000 mypy_boto3-1.34.97/mypy_boto3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:33:12.000000 mypy_boto3-1.34.97/mypy_boto3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:33:12.000000 mypy_boto3-1.34.97/mypy_boto3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 19:33:12.000000 mypy_boto3-1.34.97/mypy_boto3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 19:33:12.000000 mypy_boto3-1.34.97/mypy_boto3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:33:12.058103 mypy_boto3-1.34.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-02 19:31:52.000000 mypy_boto3-1.34.97/setup.py
```

### Comparing `mypy_boto3-1.34.96/LICENSE` & `mypy_boto3-1.34.97/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3-1.34.96/PKG-INFO` & `mypy_boto3-1.34.97/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3
-Version: 1.34.96
-Summary: Type annotations for boto3 1.34.96 master module generated with mypy-boto3-builder 7.24.0
+Version: 1.34.97
+Summary: Type annotations for boto3 1.34.97 master module generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -40,15 +40,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3)](https://pepy.tech/project/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/1.34.96/index.html)
+[boto3 1.34.97](https://boto3.amazonaws.com/v1/documentation/api/1.34.97/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
 [mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
```

### Comparing `mypy_boto3-1.34.96/README.md` & `mypy_boto3-1.34.97/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3)](https://pepy.tech/project/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/1.34.96/index.html)
+[boto3 1.34.97](https://boto3.amazonaws.com/v1/documentation/api/1.34.97/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
 [mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
```

### Comparing `mypy_boto3-1.34.96/mypy_boto3/boto3_init_stub.py` & `mypy_boto3-1.34.97/mypy_boto3/boto3_init_stub.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3-1.34.96/mypy_boto3/boto3_session_stub.py` & `mypy_boto3-1.34.97/mypy_boto3/boto3_session_stub.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3-1.34.96/mypy_boto3/literals.py` & `mypy_boto3-1.34.97/mypy_boto3/literals.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3-1.34.96/mypy_boto3/main.py` & `mypy_boto3-1.34.97/mypy_boto3/main.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3-1.34.96/mypy_boto3/submodules.py` & `mypy_boto3-1.34.97/mypy_boto3/submodules.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3-1.34.96/mypy_boto3.egg-info/PKG-INFO` & `mypy_boto3-1.34.97/mypy_boto3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3
-Version: 1.34.96
-Summary: Type annotations for boto3 1.34.96 master module generated with mypy-boto3-builder 7.24.0
+Version: 1.34.97
+Summary: Type annotations for boto3 1.34.97 master module generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -40,15 +40,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3)](https://pepy.tech/project/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/1.34.96/index.html)
+[boto3 1.34.97](https://boto3.amazonaws.com/v1/documentation/api/1.34.97/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
 [mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
```

### Comparing `mypy_boto3-1.34.96/setup.py` & `mypy_boto3-1.34.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3",
-    version="1.34.96",
+    version="1.34.97",
     packages=[
         "mypy_boto3",
     ],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3 1.34.96 master module generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3 1.34.97 master module generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

