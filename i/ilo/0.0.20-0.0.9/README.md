# Comparing `tmp/ilo-0.0.20.tar.gz` & `tmp/ilo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilo-0.0.20.tar", last modified: Thu May  2 14:28:20 2024, max compression
+gzip compressed data, was "ilo-0.0.9.tar", last modified: Thu Dec 16 12:00:24 2021, max compression
```

## Comparing `ilo-0.0.20.tar` & `ilo-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 14:28:20.989852 ilo-0.0.20/
--rw-rw-rw-   0        0        0     2156 2024-05-02 14:28:20.988845 ilo-0.0.20/PKG-INFO
--rw-rw-rw-   0        0        0     1589 2024-05-02 14:19:59.000000 ilo-0.0.20/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 14:28:20.961434 ilo-0.0.20/libname/
-drwxrwxrwx   0        0        0        0 2024-05-02 14:28:20.987441 ilo-0.0.20/libname/ilo.egg-info/
--rw-rw-rw-   0        0        0     2156 2024-05-02 14:28:20.000000 ilo-0.0.20/libname/ilo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-05-02 14:28:20.000000 ilo-0.0.20/libname/ilo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 14:28:20.000000 ilo-0.0.20/libname/ilo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 14:28:20.000000 ilo-0.0.20/libname/ilo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-02 14:28:20.000000 ilo-0.0.20/libname/ilo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    20911 2024-05-02 14:24:03.000000 ilo-0.0.20/libname/ilo.py
--rw-rw-rw-   0        0        0       42 2024-05-02 14:28:20.989852 ilo-0.0.20/setup.cfg
--rw-rw-rw-   0        0        0      936 2024-05-02 14:20:29.000000 ilo-0.0.20/setup.py
+drwxrwxrwx   0        0        0        0 2021-12-16 12:00:24.592552 ilo-0.0.9/
+-rw-rw-rw-   0        0        0      665 2021-12-16 12:00:24.592552 ilo-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2021-12-15 07:37:41.000000 ilo-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2021-12-16 12:00:24.592552 ilo-0.0.9/libname/
+drwxrwxrwx   0        0        0        0 2021-12-16 12:00:24.592552 ilo-0.0.9/libname/ilo.egg-info/
+-rw-rw-rw-   0        0        0      665 2021-12-16 12:00:24.000000 ilo-0.0.9/libname/ilo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2021-12-16 12:00:24.000000 ilo-0.0.9/libname/ilo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-12-16 12:00:24.000000 ilo-0.0.9/libname/ilo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2021-12-16 12:00:24.000000 ilo-0.0.9/libname/ilo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14837 2021-12-16 11:58:01.000000 ilo-0.0.9/libname/ilo.py
+-rw-rw-rw-   0        0        0       42 2021-12-16 12:00:24.592552 ilo-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      902 2021-12-16 12:00:18.000000 ilo-0.0.9/setup.py
```

### Comparing `ilo-0.0.20/setup.py` & `ilo-0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 from setuptools import setup
 
-VERSION = '0.0.20'
+VERSION = '0.0.9'
 DESCRIPTION = 'Control ilo robot using python command.'
-with open('README.md') as f:
-    long_description = f.read()
+LONG_DESCRIPTION = 'A package that allows user to control ilo the new education robot using python line command.'
 
 # Setting up
 setup(
     name="ilo",
     version=VERSION,
-    author="intuition RT (SLB)",
-    author_email="<contact@ilorobot.com>",
+    author="ilo robot (SLB)",
+    author_email="<ilotherobot@gmail.com>",
     url="https://github.com/ilorobot/python-library",
     description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type="text/markdown",
+    long_description=LONG_DESCRIPTION,
     py_modules=["ilo"],
     package_dir={'':'libname'},
-    install_requires=[
-        "keyboard",
-    ],
+    install_requires=[],
     keywords=['python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
-)
-
+)
```

