# Comparing `tmp/quantumz-0.0.2.tar.gz` & `tmp/quantumz-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantumz-0.0.2.tar", last modified: Thu May  2 16:50:51 2024, max compression
+gzip compressed data, was "quantumz-0.0.3.tar", last modified: Thu May  2 16:57:51 2024, max compression
```

## Comparing `quantumz-0.0.2.tar` & `quantumz-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2024-05-02 16:50:51.368594 quantumz-0.0.2/
--rw-r--r--   0 sergejzuev   (501) staff       (20)    35354 2023-07-06 05:26:58.000000 quantumz-0.0.2/LICENSE
--rw-r--r--   0 sergejzuev   (501) staff       (20)      669 2024-05-02 16:50:51.368756 quantumz-0.0.2/PKG-INFO
--rw-r--r--   0 sergejzuev   (501) staff       (20)      331 2023-07-06 05:31:18.000000 quantumz-0.0.2/README.md
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2024-05-02 16:50:51.365663 quantumz-0.0.2/quantumz/
--rwxr-xr-x   0 sergejzuev   (501) staff       (20)       19 2023-05-15 20:13:28.000000 quantumz-0.0.2/quantumz/__init__.py
--rw-r--r--   0 sergejzuev   (501) staff       (20)    16789 2024-05-02 16:26:32.000000 quantumz-0.0.2/quantumz/main.py
--rw-r--r--   0 sergejzuev   (501) staff       (20)    17510 2023-07-06 05:23:58.000000 quantumz-0.0.2/quantumz/main_old.py
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2024-05-02 16:50:51.368139 quantumz-0.0.2/quantumz.egg-info/
--rw-r--r--   0 sergejzuev   (501) staff       (20)      669 2024-05-02 16:50:51.000000 quantumz-0.0.2/quantumz.egg-info/PKG-INFO
--rw-r--r--   0 sergejzuev   (501) staff       (20)      223 2024-05-02 16:50:51.000000 quantumz-0.0.2/quantumz.egg-info/SOURCES.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2024-05-02 16:50:51.000000 quantumz-0.0.2/quantumz.egg-info/dependency_links.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)        9 2024-05-02 16:50:51.000000 quantumz-0.0.2/quantumz.egg-info/top_level.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)       38 2024-05-02 16:50:51.369372 quantumz-0.0.2/setup.cfg
--rw-r--r--   0 sergejzuev   (501) staff       (20)      506 2024-05-02 16:48:31.000000 quantumz-0.0.2/setup.py
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2024-05-02 16:57:51.592438 quantumz-0.0.3/
+-rw-r--r--   0 sergejzuev   (501) staff       (20)    35354 2023-07-06 05:26:58.000000 quantumz-0.0.3/LICENSE
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      669 2024-05-02 16:57:51.592706 quantumz-0.0.3/PKG-INFO
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      331 2023-07-06 05:31:18.000000 quantumz-0.0.3/README.md
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2024-05-02 16:57:51.587176 quantumz-0.0.3/quantumz/
+-rwxr-xr-x   0 sergejzuev   (501) staff       (20)       19 2023-05-15 20:13:28.000000 quantumz-0.0.3/quantumz/__init__.py
+-rw-r--r--   0 sergejzuev   (501) staff       (20)    16803 2024-05-02 16:54:45.000000 quantumz-0.0.3/quantumz/main.py
+-rw-r--r--   0 sergejzuev   (501) staff       (20)    17510 2023-07-06 05:23:58.000000 quantumz-0.0.3/quantumz/main_old.py
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2024-05-02 16:57:51.591788 quantumz-0.0.3/quantumz.egg-info/
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      669 2024-05-02 16:57:51.000000 quantumz-0.0.3/quantumz.egg-info/PKG-INFO
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      223 2024-05-02 16:57:51.000000 quantumz-0.0.3/quantumz.egg-info/SOURCES.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2024-05-02 16:57:51.000000 quantumz-0.0.3/quantumz.egg-info/dependency_links.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)        9 2024-05-02 16:57:51.000000 quantumz-0.0.3/quantumz.egg-info/top_level.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)       38 2024-05-02 16:57:51.593526 quantumz-0.0.3/setup.cfg
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      506 2024-05-02 16:57:26.000000 quantumz-0.0.3/setup.py
```

### Comparing `quantumz-0.0.2/LICENSE` & `quantumz-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quantumz-0.0.2/PKG-INFO` & `quantumz-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantumz
-Version: 0.0.2
+Version: 0.0.3
 Summary: A module for quantum computing emulations
 Author: Sergei Zuev
 Author-email: shoukhov@mail.ru
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `quantumz-0.0.2/quantumz/main.py` & `quantumz-0.0.3/quantumz/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -599,21 +599,21 @@
         q (dict): a quantum state
         t (int): number of registers under action
 
     Returns
     -------
         The resulted quantum state
     """ 
-   n = len(list(q.keys())[0])-2
-   m = n-t
-   rq = {}
-   for k in q.keys():
-       a = q[k]
-       kr = k[:t+1]+'>'
-       u = U({kr:1})
-       for ku in u.keys():
-           kur = ku[:-1]+k[t+1:]
-           if kur in rq:
-               rq[kur] += u[ku]*a
-           else:
-               rq[kur] = u[ku]*a
-   return rq
+    n = len(list(q.keys())[0])-2
+    m = n-t
+    rq = {}
+    for k in q.keys():
+        a = q[k]
+        kr = k[:t+1]+'>'
+        u = U({kr:1})
+        for ku in u.keys():
+            kur = ku[:-1]+k[t+1:]
+            if kur in rq:
+                rq[kur] += u[ku]*a
+            else:
+                rq[kur] = u[ku]*a
+    return rq
```

### Comparing `quantumz-0.0.2/quantumz/main_old.py` & `quantumz-0.0.3/quantumz/main_old.py`

 * *Files identical despite different names*

### Comparing `quantumz-0.0.2/quantumz.egg-info/PKG-INFO` & `quantumz-0.0.3/quantumz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantumz
-Version: 0.0.2
+Version: 0.0.3
 Summary: A module for quantum computing emulations
 Author: Sergei Zuev
 Author-email: shoukhov@mail.ru
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

