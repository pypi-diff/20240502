# Comparing `tmp/quantumz-0.0.3.tar.gz` & `tmp/quantumz-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantumz-0.0.3.tar", last modified: Thu May  2 16:57:51 2024, max compression
+gzip compressed data, was "quantumz-0.0.4.tar", last modified: Thu May  2 17:02:05 2024, max compression
```

## Comparing `quantumz-0.0.3.tar` & `quantumz-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2024-05-02 16:57:51.592438 quantumz-0.0.3/
--rw-r--r--   0 sergejzuev   (501) staff       (20)    35354 2023-07-06 05:26:58.000000 quantumz-0.0.3/LICENSE
--rw-r--r--   0 sergejzuev   (501) staff       (20)      669 2024-05-02 16:57:51.592706 quantumz-0.0.3/PKG-INFO
--rw-r--r--   0 sergejzuev   (501) staff       (20)      331 2023-07-06 05:31:18.000000 quantumz-0.0.3/README.md
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2024-05-02 16:57:51.587176 quantumz-0.0.3/quantumz/
--rwxr-xr-x   0 sergejzuev   (501) staff       (20)       19 2023-05-15 20:13:28.000000 quantumz-0.0.3/quantumz/__init__.py
--rw-r--r--   0 sergejzuev   (501) staff       (20)    16803 2024-05-02 16:54:45.000000 quantumz-0.0.3/quantumz/main.py
--rw-r--r--   0 sergejzuev   (501) staff       (20)    17510 2023-07-06 05:23:58.000000 quantumz-0.0.3/quantumz/main_old.py
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2024-05-02 16:57:51.591788 quantumz-0.0.3/quantumz.egg-info/
--rw-r--r--   0 sergejzuev   (501) staff       (20)      669 2024-05-02 16:57:51.000000 quantumz-0.0.3/quantumz.egg-info/PKG-INFO
--rw-r--r--   0 sergejzuev   (501) staff       (20)      223 2024-05-02 16:57:51.000000 quantumz-0.0.3/quantumz.egg-info/SOURCES.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2024-05-02 16:57:51.000000 quantumz-0.0.3/quantumz.egg-info/dependency_links.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)        9 2024-05-02 16:57:51.000000 quantumz-0.0.3/quantumz.egg-info/top_level.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)       38 2024-05-02 16:57:51.593526 quantumz-0.0.3/setup.cfg
--rw-r--r--   0 sergejzuev   (501) staff       (20)      506 2024-05-02 16:57:26.000000 quantumz-0.0.3/setup.py
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2024-05-02 17:02:05.224941 quantumz-0.0.4/
+-rw-r--r--   0 sergejzuev   (501) staff       (20)    35354 2023-07-06 05:26:58.000000 quantumz-0.0.4/LICENSE
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      669 2024-05-02 17:02:05.225255 quantumz-0.0.4/PKG-INFO
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      331 2023-07-06 05:31:18.000000 quantumz-0.0.4/README.md
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2024-05-02 17:02:05.218356 quantumz-0.0.4/quantumz/
+-rwxr-xr-x   0 sergejzuev   (501) staff       (20)       19 2023-05-15 20:13:28.000000 quantumz-0.0.4/quantumz/__init__.py
+-rw-r--r--   0 sergejzuev   (501) staff       (20)    16803 2024-05-02 17:01:31.000000 quantumz-0.0.4/quantumz/main.py
+-rw-r--r--   0 sergejzuev   (501) staff       (20)    17510 2023-07-06 05:23:58.000000 quantumz-0.0.4/quantumz/main_old.py
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2024-05-02 17:02:05.224227 quantumz-0.0.4/quantumz.egg-info/
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      669 2024-05-02 17:02:04.000000 quantumz-0.0.4/quantumz.egg-info/PKG-INFO
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      223 2024-05-02 17:02:05.000000 quantumz-0.0.4/quantumz.egg-info/SOURCES.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2024-05-02 17:02:04.000000 quantumz-0.0.4/quantumz.egg-info/dependency_links.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)        9 2024-05-02 17:02:04.000000 quantumz-0.0.4/quantumz.egg-info/top_level.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)       38 2024-05-02 17:02:05.226183 quantumz-0.0.4/setup.cfg
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      506 2024-05-02 17:00:31.000000 quantumz-0.0.4/setup.py
```

### Comparing `quantumz-0.0.3/LICENSE` & `quantumz-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quantumz-0.0.3/PKG-INFO` & `quantumz-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantumz
-Version: 0.0.3
+Version: 0.0.4
 Summary: A module for quantum computing emulations
 Author: Sergei Zuev
 Author-email: shoukhov@mail.ru
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `quantumz-0.0.3/quantumz/main.py` & `quantumz-0.0.4/quantumz/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -585,21 +585,21 @@
     -------
         Complete superposition quantum state
     """
     q = initq(n)
     for i in range(n):
         q = H(q,i)
     return q
-def partially(Ug: func, q: dict, t: int): 
+def partially(Ug: dict, q: dict, t: int): 
     """
     Ug gate acts on the first n registers of the quantum state q.
 
     Parameters
     ----------
-        Ug (func): a n-dimensional quantum gate
+        Ug (dict): a n-dimensional quantum gate
         q (dict): a quantum state
         t (int): number of registers under action
 
     Returns
     -------
         The resulted quantum state
     """
```

### Comparing `quantumz-0.0.3/quantumz/main_old.py` & `quantumz-0.0.4/quantumz/main_old.py`

 * *Files identical despite different names*

### Comparing `quantumz-0.0.3/quantumz.egg-info/PKG-INFO` & `quantumz-0.0.4/quantumz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantumz
-Version: 0.0.3
+Version: 0.0.4
 Summary: A module for quantum computing emulations
 Author: Sergei Zuev
 Author-email: shoukhov@mail.ru
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

