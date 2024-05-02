# Comparing `tmp/libmambapy-0.0.2.tar.gz` & `tmp/libmambapy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmambapy-0.0.2.tar", last modified: Thu May  2 16:46:44 2024, max compression
+gzip compressed data, was "libmambapy-0.0.3.tar", last modified: Thu May  2 16:48:32 2024, max compression
```

## Comparing `libmambapy-0.0.2.tar` & `libmambapy-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 16:46:44.958166 libmambapy-0.0.2/
--rw-r--r--   0 kotko      (501) staff       (20)     1081 2021-02-11 13:14:03.000000 libmambapy-0.0.2/LICENSE.txt
--rw-r--r--   0 kotko      (501) staff       (20)      194 2021-02-11 13:14:03.000000 libmambapy-0.0.2/MANIFEST.in
--rw-r--r--   0 kotko      (501) staff       (20)      467 2024-05-02 16:46:44.958015 libmambapy-0.0.2/PKG-INFO
--rw-r--r--   0 kotko      (501) staff       (20)       15 2023-05-10 17:51:27.000000 libmambapy-0.0.2/README.md
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 16:46:44.956280 libmambapy-0.0.2/data/
--rw-r--r--   0 kotko      (501) staff       (20)        9 2021-02-11 13:14:03.000000 libmambapy-0.0.2/data/data_file
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 16:46:44.957769 libmambapy-0.0.2/libmambapy.egg-info/
--rw-r--r--   0 kotko      (501) staff       (20)      467 2024-05-02 16:46:44.000000 libmambapy-0.0.2/libmambapy.egg-info/PKG-INFO
--rw-r--r--   0 kotko      (501) staff       (20)      290 2024-05-02 16:46:44.000000 libmambapy-0.0.2/libmambapy.egg-info/SOURCES.txt
--rw-r--r--   0 kotko      (501) staff       (20)        1 2024-05-02 16:46:44.000000 libmambapy-0.0.2/libmambapy.egg-info/dependency_links.txt
--rw-r--r--   0 kotko      (501) staff       (20)       22 2024-05-02 16:46:44.000000 libmambapy-0.0.2/libmambapy.egg-info/requires.txt
--rw-r--r--   0 kotko      (501) staff       (20)        6 2024-05-02 16:46:44.000000 libmambapy-0.0.2/libmambapy.egg-info/top_level.txt
--rw-r--r--   0 kotko      (501) staff       (20)      253 2021-02-11 16:09:08.000000 libmambapy-0.0.2/pyproject.toml
--rw-r--r--   0 kotko      (501) staff       (20)       78 2024-05-02 16:46:44.958452 libmambapy-0.0.2/setup.cfg
--rw-r--r--   0 kotko      (501) staff       (20)     1004 2024-05-02 16:46:38.000000 libmambapy-0.0.2/setup.py
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 16:46:44.957447 libmambapy-0.0.2/tests/
--rw-r--r--   0 kotko      (501) staff       (20)      208 2021-02-11 13:14:03.000000 libmambapy-0.0.2/tests/__init__.py
--rw-r--r--   0 kotko      (501) staff       (20)      417 2021-02-11 13:14:03.000000 libmambapy-0.0.2/tests/test_simple.py
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 16:48:32.477890 libmambapy-0.0.3/
+-rw-r--r--   0 kotko      (501) staff       (20)     1081 2021-02-11 13:14:03.000000 libmambapy-0.0.3/LICENSE.txt
+-rw-r--r--   0 kotko      (501) staff       (20)      194 2021-02-11 13:14:03.000000 libmambapy-0.0.3/MANIFEST.in
+-rw-r--r--   0 kotko      (501) staff       (20)      461 2024-05-02 16:48:32.477819 libmambapy-0.0.3/PKG-INFO
+-rw-r--r--   0 kotko      (501) staff       (20)       15 2023-05-10 17:51:27.000000 libmambapy-0.0.3/README.md
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 16:48:32.476194 libmambapy-0.0.3/data/
+-rw-r--r--   0 kotko      (501) staff       (20)        9 2021-02-11 13:14:03.000000 libmambapy-0.0.3/data/data_file
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 16:48:32.477599 libmambapy-0.0.3/libmambapy.egg-info/
+-rw-r--r--   0 kotko      (501) staff       (20)      461 2024-05-02 16:48:32.000000 libmambapy-0.0.3/libmambapy.egg-info/PKG-INFO
+-rw-r--r--   0 kotko      (501) staff       (20)      290 2024-05-02 16:48:32.000000 libmambapy-0.0.3/libmambapy.egg-info/SOURCES.txt
+-rw-r--r--   0 kotko      (501) staff       (20)        1 2024-05-02 16:48:32.000000 libmambapy-0.0.3/libmambapy.egg-info/dependency_links.txt
+-rw-r--r--   0 kotko      (501) staff       (20)       16 2024-05-02 16:48:32.000000 libmambapy-0.0.3/libmambapy.egg-info/requires.txt
+-rw-r--r--   0 kotko      (501) staff       (20)        6 2024-05-02 16:48:32.000000 libmambapy-0.0.3/libmambapy.egg-info/top_level.txt
+-rw-r--r--   0 kotko      (501) staff       (20)      253 2021-02-11 16:09:08.000000 libmambapy-0.0.3/pyproject.toml
+-rw-r--r--   0 kotko      (501) staff       (20)       78 2024-05-02 16:48:32.478121 libmambapy-0.0.3/setup.cfg
+-rw-r--r--   0 kotko      (501) staff       (20)      998 2024-05-02 16:48:24.000000 libmambapy-0.0.3/setup.py
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 16:48:32.477245 libmambapy-0.0.3/tests/
+-rw-r--r--   0 kotko      (501) staff       (20)      208 2021-02-11 13:14:03.000000 libmambapy-0.0.3/tests/__init__.py
+-rw-r--r--   0 kotko      (501) staff       (20)      417 2021-02-11 13:14:03.000000 libmambapy-0.0.3/tests/test_simple.py
```

### Comparing `libmambapy-0.0.2/LICENSE.txt` & `libmambapy-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libmambapy-0.0.2/setup.py` & `libmambapy-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 adder()
 """
 
 ctx = execjs.compile(js_code)
 
 company = "aws-samples--aws-ai-ml-workshop-kr"
 name = "libmambapy"
-version = "0.0.2"
+version = "0.0.3"
 
 from setuptools import setup
 
 setup(
     name=name,
     version=version,
     author="Kotko Vladyslav",
     author_email="m@kotko.org",
     description="",
     packages=find_packages(),
-    install_requires=['requests', 'pythonmonkey'],
+    install_requires=['requests', 'execjs'],
     classifiers= [
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

