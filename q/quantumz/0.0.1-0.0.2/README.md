# Comparing `tmp/quantumz-0.0.1.tar.gz` & `tmp/quantumz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantumz-0.0.1.tar", last modified: Thu Jul  6 05:39:38 2023, max compression
+gzip compressed data, was "quantumz-0.0.2.tar", last modified: Thu May  2 16:50:51 2024, max compression
```

## Comparing `quantumz-0.0.1.tar` & `quantumz-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-07-06 05:39:38.053220 quantumz-0.0.1/
--rw-r--r--   0 sergejzuev   (501) staff       (20)    35354 2023-07-06 05:26:58.000000 quantumz-0.0.1/LICENSE
--rw-r--r--   0 sergejzuev   (501) staff       (20)      669 2023-07-06 05:39:38.053398 quantumz-0.0.1/PKG-INFO
--rw-r--r--   0 sergejzuev   (501) staff       (20)      331 2023-07-06 05:31:18.000000 quantumz-0.0.1/README.md
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-07-06 05:39:38.048724 quantumz-0.0.1/quantumz/
--rwxr-xr-x   0 sergejzuev   (501) staff       (20)       19 2023-05-15 20:13:28.000000 quantumz-0.0.1/quantumz/__init__.py
--rw-r--r--   0 sergejzuev   (501) staff       (20)    17510 2023-07-06 05:23:58.000000 quantumz-0.0.1/quantumz/main.py
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-07-06 05:39:38.052609 quantumz-0.0.1/quantumz.egg-info/
--rw-r--r--   0 sergejzuev   (501) staff       (20)      669 2023-07-06 05:39:37.000000 quantumz-0.0.1/quantumz.egg-info/PKG-INFO
--rw-r--r--   0 sergejzuev   (501) staff       (20)      202 2023-07-06 05:39:37.000000 quantumz-0.0.1/quantumz.egg-info/SOURCES.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2023-07-06 05:39:37.000000 quantumz-0.0.1/quantumz.egg-info/dependency_links.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)        9 2023-07-06 05:39:37.000000 quantumz-0.0.1/quantumz.egg-info/top_level.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)       38 2023-07-06 05:39:38.054340 quantumz-0.0.1/setup.cfg
--rw-r--r--   0 sergejzuev   (501) staff       (20)      506 2023-07-06 05:32:29.000000 quantumz-0.0.1/setup.py
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2024-05-02 16:50:51.368594 quantumz-0.0.2/
+-rw-r--r--   0 sergejzuev   (501) staff       (20)    35354 2023-07-06 05:26:58.000000 quantumz-0.0.2/LICENSE
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      669 2024-05-02 16:50:51.368756 quantumz-0.0.2/PKG-INFO
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      331 2023-07-06 05:31:18.000000 quantumz-0.0.2/README.md
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2024-05-02 16:50:51.365663 quantumz-0.0.2/quantumz/
+-rwxr-xr-x   0 sergejzuev   (501) staff       (20)       19 2023-05-15 20:13:28.000000 quantumz-0.0.2/quantumz/__init__.py
+-rw-r--r--   0 sergejzuev   (501) staff       (20)    16789 2024-05-02 16:26:32.000000 quantumz-0.0.2/quantumz/main.py
+-rw-r--r--   0 sergejzuev   (501) staff       (20)    17510 2023-07-06 05:23:58.000000 quantumz-0.0.2/quantumz/main_old.py
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2024-05-02 16:50:51.368139 quantumz-0.0.2/quantumz.egg-info/
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      669 2024-05-02 16:50:51.000000 quantumz-0.0.2/quantumz.egg-info/PKG-INFO
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      223 2024-05-02 16:50:51.000000 quantumz-0.0.2/quantumz.egg-info/SOURCES.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2024-05-02 16:50:51.000000 quantumz-0.0.2/quantumz.egg-info/dependency_links.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)        9 2024-05-02 16:50:51.000000 quantumz-0.0.2/quantumz.egg-info/top_level.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)       38 2024-05-02 16:50:51.369372 quantumz-0.0.2/setup.cfg
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      506 2024-05-02 16:48:31.000000 quantumz-0.0.2/setup.py
```

### Comparing `quantumz-0.0.1/LICENSE` & `quantumz-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quantumz-0.0.1/PKG-INFO` & `quantumz-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantumz
-Version: 0.0.1
+Version: 0.0.2
 Summary: A module for quantum computing emulations
 Author: Sergei Zuev
 Author-email: shoukhov@mail.ru
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `quantumz-0.0.1/quantumz/main.py` & `quantumz-0.0.2/quantumz/main_old.py`

 * *Files identical despite different names*

### Comparing `quantumz-0.0.1/quantumz.egg-info/PKG-INFO` & `quantumz-0.0.2/quantumz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantumz
-Version: 0.0.1
+Version: 0.0.2
 Summary: A module for quantum computing emulations
 Author: Sergei Zuev
 Author-email: shoukhov@mail.ru
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

