# Comparing `tmp/shodo-0.0.8.tar.gz` & `tmp/shodo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shodo-0.0.8.tar", last modified: Wed Jan 18 06:49:12 2023, max compression
+gzip compressed data, was "shodo-0.0.9.tar", last modified: Mon Feb  6 06:20:57 2023, max compression
```

## Comparing `shodo-0.0.8.tar` & `shodo-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 hirokiky  (1000) hirokiky  (1000)        0 2023-01-18 06:49:12.549827 shodo-0.0.8/
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1073 2022-05-18 01:55:00.000000 shodo-0.0.8/LICENSE
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1793 2023-01-18 06:49:12.549827 shodo-0.0.8/PKG-INFO
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1399 2022-08-02 06:32:16.000000 shodo-0.0.8/README.md
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)       38 2023-01-18 06:49:12.549827 shodo-0.0.8/setup.cfg
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      797 2023-01-18 06:47:43.000000 shodo-0.0.8/setup.py
-drwxrwxr-x   0 hirokiky  (1000) hirokiky  (1000)        0 2023-01-18 06:49:12.545827 shodo-0.0.8/shodo/
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)       50 2022-05-18 00:58:25.000000 shodo-0.0.8/shodo/__init__.py
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1326 2022-08-02 05:23:14.000000 shodo-0.0.8/shodo/api.py
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1242 2022-09-29 01:51:49.000000 shodo-0.0.8/shodo/conf.py
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1589 2022-12-15 07:19:05.000000 shodo-0.0.8/shodo/lint.py
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     2341 2023-01-18 06:39:59.000000 shodo-0.0.8/shodo/main.py
-drwxrwxr-x   0 hirokiky  (1000) hirokiky  (1000)        0 2023-01-18 06:49:12.549827 shodo-0.0.8/shodo.egg-info/
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1793 2023-01-18 06:49:12.000000 shodo-0.0.8/shodo.egg-info/PKG-INFO
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      275 2023-01-18 06:49:12.000000 shodo-0.0.8/shodo.egg-info/SOURCES.txt
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)        1 2023-01-18 06:49:12.000000 shodo-0.0.8/shodo.egg-info/dependency_links.txt
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)       42 2023-01-18 06:49:12.000000 shodo-0.0.8/shodo.egg-info/entry_points.txt
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)       15 2023-01-18 06:49:12.000000 shodo-0.0.8/shodo.egg-info/requires.txt
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)        6 2023-01-18 06:49:12.000000 shodo-0.0.8/shodo.egg-info/top_level.txt
+drwxrwxr-x   0 hirokiky  (1000) hirokiky  (1000)        0 2023-02-06 06:20:57.966913 shodo-0.0.9/
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1073 2022-05-18 01:55:00.000000 shodo-0.0.9/LICENSE
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1793 2023-02-06 06:20:57.966913 shodo-0.0.9/PKG-INFO
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1399 2022-08-02 06:32:16.000000 shodo-0.0.9/README.md
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)       38 2023-02-06 06:20:57.966913 shodo-0.0.9/setup.cfg
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      797 2023-02-06 06:19:51.000000 shodo-0.0.9/setup.py
+drwxrwxr-x   0 hirokiky  (1000) hirokiky  (1000)        0 2023-02-06 06:20:57.966913 shodo-0.0.9/shodo/
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)       50 2022-05-18 00:58:25.000000 shodo-0.0.9/shodo/__init__.py
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1326 2022-08-02 05:23:14.000000 shodo-0.0.9/shodo/api.py
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1242 2022-09-29 01:51:49.000000 shodo-0.0.9/shodo/conf.py
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1603 2023-02-06 06:19:35.000000 shodo-0.0.9/shodo/lint.py
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     2341 2023-01-18 06:39:59.000000 shodo-0.0.9/shodo/main.py
+drwxrwxr-x   0 hirokiky  (1000) hirokiky  (1000)        0 2023-02-06 06:20:57.966913 shodo-0.0.9/shodo.egg-info/
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1793 2023-02-06 06:20:57.000000 shodo-0.0.9/shodo.egg-info/PKG-INFO
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      275 2023-02-06 06:20:57.000000 shodo-0.0.9/shodo.egg-info/SOURCES.txt
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)        1 2023-02-06 06:20:57.000000 shodo-0.0.9/shodo.egg-info/dependency_links.txt
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)       42 2023-02-06 06:20:57.000000 shodo-0.0.9/shodo.egg-info/entry_points.txt
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)       15 2023-02-06 06:20:57.000000 shodo-0.0.9/shodo.egg-info/requires.txt
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)        6 2023-02-06 06:20:57.000000 shodo-0.0.9/shodo.egg-info/top_level.txt
```

### Comparing `shodo-0.0.8/LICENSE` & `shodo-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shodo-0.0.8/PKG-INFO` & `shodo-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shodo
-Version: 0.0.8
+Version: 0.0.9
 Summary: Shodo Python CLI
 Home-page: https://github.com/zenproducts/shodo-python
 Author: ZenProducts Inc.
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `shodo-0.0.8/README.md` & `shodo-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `shodo-0.0.8/setup.py` & `shodo-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, "README.md")).read()
 
 
 setup(
     name="shodo",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(),
     url="https://github.com/zenproducts/shodo-python",
     license="MIT",
     author="ZenProducts Inc.",
     description="Shodo Python CLI",
     long_description=README,
     long_description_content_type="text/markdown",
```

### Comparing `shodo-0.0.8/shodo/api.py` & `shodo-0.0.9/shodo/api.py`

 * *Files identical despite different names*

### Comparing `shodo-0.0.8/shodo/conf.py` & `shodo-0.0.9/shodo/conf.py`

 * *Files identical despite different names*

### Comparing `shodo-0.0.8/shodo/lint.py` & `shodo-0.0.9/shodo/lint.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 
 @dataclass
 class Message:
     ERROR = "error"
     WARNING = "warning"
 
+    code: str
     message: str
     severity: str
     from_: Pos
     to: Pos
     index: int
     index_to: int
     score: float
```

### Comparing `shodo-0.0.8/shodo/main.py` & `shodo-0.0.9/shodo/main.py`

 * *Files identical despite different names*

### Comparing `shodo-0.0.8/shodo.egg-info/PKG-INFO` & `shodo-0.0.9/shodo.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shodo
-Version: 0.0.8
+Version: 0.0.9
 Summary: Shodo Python CLI
 Home-page: https://github.com/zenproducts/shodo-python
 Author: ZenProducts Inc.
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

