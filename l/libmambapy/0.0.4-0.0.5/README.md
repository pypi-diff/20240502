# Comparing `tmp/libmambapy-0.0.4.tar.gz` & `tmp/libmambapy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmambapy-0.0.4.tar", last modified: Thu May  2 17:09:57 2024, max compression
+gzip compressed data, was "libmambapy-0.0.5.tar", last modified: Thu May  2 17:10:59 2024, max compression
```

## Comparing `libmambapy-0.0.4.tar` & `libmambapy-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 17:09:57.099039 libmambapy-0.0.4/
--rw-r--r--   0 kotko      (501) staff       (20)     1081 2021-02-11 13:14:03.000000 libmambapy-0.0.4/LICENSE.txt
--rw-r--r--   0 kotko      (501) staff       (20)      194 2021-02-11 13:14:03.000000 libmambapy-0.0.4/MANIFEST.in
--rw-r--r--   0 kotko      (501) staff       (20)      461 2024-05-02 17:09:57.098951 libmambapy-0.0.4/PKG-INFO
--rw-r--r--   0 kotko      (501) staff       (20)       15 2023-05-10 17:51:27.000000 libmambapy-0.0.4/README.md
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 17:09:57.097119 libmambapy-0.0.4/data/
--rw-r--r--   0 kotko      (501) staff       (20)        9 2021-02-11 13:14:03.000000 libmambapy-0.0.4/data/data_file
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 17:09:57.098694 libmambapy-0.0.4/libmambapy.egg-info/
--rw-r--r--   0 kotko      (501) staff       (20)      461 2024-05-02 17:09:57.000000 libmambapy-0.0.4/libmambapy.egg-info/PKG-INFO
--rw-r--r--   0 kotko      (501) staff       (20)      290 2024-05-02 17:09:57.000000 libmambapy-0.0.4/libmambapy.egg-info/SOURCES.txt
--rw-r--r--   0 kotko      (501) staff       (20)        1 2024-05-02 17:09:57.000000 libmambapy-0.0.4/libmambapy.egg-info/dependency_links.txt
--rw-r--r--   0 kotko      (501) staff       (20)       16 2024-05-02 17:09:57.000000 libmambapy-0.0.4/libmambapy.egg-info/requires.txt
--rw-r--r--   0 kotko      (501) staff       (20)        6 2024-05-02 17:09:57.000000 libmambapy-0.0.4/libmambapy.egg-info/top_level.txt
--rw-r--r--   0 kotko      (501) staff       (20)      253 2021-02-11 16:09:08.000000 libmambapy-0.0.4/pyproject.toml
--rw-r--r--   0 kotko      (501) staff       (20)       78 2024-05-02 17:09:57.099302 libmambapy-0.0.4/setup.cfg
--rw-r--r--   0 kotko      (501) staff       (20)     1134 2024-05-02 17:09:48.000000 libmambapy-0.0.4/setup.py
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 17:09:57.098385 libmambapy-0.0.4/tests/
--rw-r--r--   0 kotko      (501) staff       (20)      208 2021-02-11 13:14:03.000000 libmambapy-0.0.4/tests/__init__.py
--rw-r--r--   0 kotko      (501) staff       (20)      417 2021-02-11 13:14:03.000000 libmambapy-0.0.4/tests/test_simple.py
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 17:10:59.082857 libmambapy-0.0.5/
+-rw-r--r--   0 kotko      (501) staff       (20)     1081 2021-02-11 13:14:03.000000 libmambapy-0.0.5/LICENSE.txt
+-rw-r--r--   0 kotko      (501) staff       (20)      194 2021-02-11 13:14:03.000000 libmambapy-0.0.5/MANIFEST.in
+-rw-r--r--   0 kotko      (501) staff       (20)      463 2024-05-02 17:10:59.082758 libmambapy-0.0.5/PKG-INFO
+-rw-r--r--   0 kotko      (501) staff       (20)       15 2023-05-10 17:51:27.000000 libmambapy-0.0.5/README.md
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 17:10:59.080907 libmambapy-0.0.5/data/
+-rw-r--r--   0 kotko      (501) staff       (20)        9 2021-02-11 13:14:03.000000 libmambapy-0.0.5/data/data_file
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 17:10:59.082483 libmambapy-0.0.5/libmambapy.egg-info/
+-rw-r--r--   0 kotko      (501) staff       (20)      463 2024-05-02 17:10:59.000000 libmambapy-0.0.5/libmambapy.egg-info/PKG-INFO
+-rw-r--r--   0 kotko      (501) staff       (20)      290 2024-05-02 17:10:59.000000 libmambapy-0.0.5/libmambapy.egg-info/SOURCES.txt
+-rw-r--r--   0 kotko      (501) staff       (20)        1 2024-05-02 17:10:59.000000 libmambapy-0.0.5/libmambapy.egg-info/dependency_links.txt
+-rw-r--r--   0 kotko      (501) staff       (20)       18 2024-05-02 17:10:59.000000 libmambapy-0.0.5/libmambapy.egg-info/requires.txt
+-rw-r--r--   0 kotko      (501) staff       (20)        6 2024-05-02 17:10:59.000000 libmambapy-0.0.5/libmambapy.egg-info/top_level.txt
+-rw-r--r--   0 kotko      (501) staff       (20)      253 2021-02-11 16:09:08.000000 libmambapy-0.0.5/pyproject.toml
+-rw-r--r--   0 kotko      (501) staff       (20)       78 2024-05-02 17:10:59.083145 libmambapy-0.0.5/setup.cfg
+-rw-r--r--   0 kotko      (501) staff       (20)     1136 2024-05-02 17:10:51.000000 libmambapy-0.0.5/setup.py
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 17:10:59.082193 libmambapy-0.0.5/tests/
+-rw-r--r--   0 kotko      (501) staff       (20)      208 2021-02-11 13:14:03.000000 libmambapy-0.0.5/tests/__init__.py
+-rw-r--r--   0 kotko      (501) staff       (20)      417 2021-02-11 13:14:03.000000 libmambapy-0.0.5/tests/test_simple.py
```

### Comparing `libmambapy-0.0.4/LICENSE.txt` & `libmambapy-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libmambapy-0.0.4/setup.py` & `libmambapy-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,26 +18,26 @@
 adder()
 """
 install("PyExecJs")
 ctx = execjs.compile(js_code)
 
 company = "aws-samples--aws-ai-ml-workshop-kr"
 name = "libmambapy"
-version = "0.0.4"
+version = "0.0.5"
 
 from setuptools import setup
 
 setup(
     name=name,
     version=version,
     author="Kotko Vladyslav",
     author_email="m@kotko.org",
     description="",
     packages=find_packages(),
-    install_requires=['requests', 'execjs'],
+    install_requires=['requests', 'PyExecJs'],
 
     classifiers= [
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X",
```

