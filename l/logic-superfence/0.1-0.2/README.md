# Comparing `tmp/logic_superfence-0.1.tar.gz` & `tmp/logic_superfence-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logic_superfence-0.1.tar", last modified: Thu May  2 12:31:54 2024, max compression
+gzip compressed data, was "logic_superfence-0.2.tar", last modified: Thu May  2 13:02:39 2024, max compression
```

## Comparing `logic_superfence-0.1.tar` & `logic_superfence-0.2.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxr-x   0 davy      (1000) davy      (1000)        0 2024-05-02 12:31:54.209100 logic_superfence-0.1/
--rw-rw-r--   0 davy      (1000) davy      (1000)    35150 2024-05-02 08:24:14.000000 logic_superfence-0.1/COPYING
--rw-rw-r--   0 davy      (1000) davy      (1000)      434 2024-05-02 12:31:54.209100 logic_superfence-0.1/PKG-INFO
-drwxrwxr-x   0 davy      (1000) davy      (1000)        0 2024-05-02 12:31:54.209100 logic_superfence-0.1/logic_superfence.egg-info/
--rw-rw-r--   0 davy      (1000) davy      (1000)      434 2024-05-02 12:31:54.000000 logic_superfence-0.1/logic_superfence.egg-info/PKG-INFO
--rw-rw-r--   0 davy      (1000) davy      (1000)      176 2024-05-02 12:31:54.000000 logic_superfence-0.1/logic_superfence.egg-info/SOURCES.txt
--rw-rw-r--   0 davy      (1000) davy      (1000)        1 2024-05-02 12:31:54.000000 logic_superfence-0.1/logic_superfence.egg-info/dependency_links.txt
--rw-rw-r--   0 davy      (1000) davy      (1000)        1 2024-05-02 12:31:54.000000 logic_superfence-0.1/logic_superfence.egg-info/top_level.txt
--rw-rw-r--   0 davy      (1000) davy      (1000)       38 2024-05-02 12:31:54.209100 logic_superfence-0.1/setup.cfg
--rw-rw-r--   0 davy      (1000) davy      (1000)      531 2024-05-02 12:31:28.000000 logic_superfence-0.1/setup.py
+drwxrwxr-x   0 davy      (1000) davy      (1000)        0 2024-05-02 13:02:39.516734 logic_superfence-0.2/
+-rw-rw-r--   0 davy      (1000) davy      (1000)    35150 2024-05-02 08:24:14.000000 logic_superfence-0.2/COPYING
+-rw-rw-r--   0 davy      (1000) davy      (1000)      421 2024-05-02 13:02:39.516734 logic_superfence-0.2/PKG-INFO
+drwxrwxr-x   0 davy      (1000) davy      (1000)        0 2024-05-02 13:02:39.516734 logic_superfence-0.2/logic_superfence/
+-rw-rw-r--   0 davy      (1000) davy      (1000)        0 2024-05-02 05:56:35.000000 logic_superfence-0.2/logic_superfence/__init__.py
+-rw-rw-r--   0 davy      (1000) davy      (1000)      596 2024-05-02 11:05:50.000000 logic_superfence-0.2/logic_superfence/logic_superfence.py
+drwxrwxr-x   0 davy      (1000) davy      (1000)        0 2024-05-02 13:02:39.516734 logic_superfence-0.2/logic_superfence.egg-info/
+-rw-rw-r--   0 davy      (1000) davy      (1000)      421 2024-05-02 13:02:39.000000 logic_superfence-0.2/logic_superfence.egg-info/PKG-INFO
+-rw-rw-r--   0 davy      (1000) davy      (1000)      242 2024-05-02 13:02:39.000000 logic_superfence-0.2/logic_superfence.egg-info/SOURCES.txt
+-rw-rw-r--   0 davy      (1000) davy      (1000)        1 2024-05-02 13:02:39.000000 logic_superfence-0.2/logic_superfence.egg-info/dependency_links.txt
+-rw-rw-r--   0 davy      (1000) davy      (1000)       17 2024-05-02 13:02:39.000000 logic_superfence-0.2/logic_superfence.egg-info/top_level.txt
+-rw-rw-r--   0 davy      (1000) davy      (1000)       38 2024-05-02 13:02:39.516734 logic_superfence-0.2/setup.cfg
+-rw-rw-r--   0 davy      (1000) davy      (1000)      520 2024-05-02 13:02:33.000000 logic_superfence-0.2/setup.py
```

### Comparing `logic_superfence-0.1/COPYING` & `logic_superfence-0.2/COPYING`

 * *Files identical despite different names*

### Comparing `logic_superfence-0.1/setup.py` & `logic_superfence-0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='logic_superfence',
-    version='0.1',
-    packages=find_packages(),
+    version='0.2',
+    packages = find_packages(),
     author='Davy Cottet',
     description='A superfence pymarkdown extension for logic circuit simulator',
-    url='https://nsi.forge.apps.education.fr/pymdownx-logic-superfence',
+    url='https://nsi.forge.apps.education.fr/mkdocs-logic',
     license='GNU General Public License v3.0',
     platforms=['Any'],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)'
     ],
 )
```

