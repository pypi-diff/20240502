# Comparing `tmp/zern-0.0.1.tar.gz` & `tmp/zern-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zern-0.0.1.tar", last modified: Thu May  2 17:58:39 2024, max compression
+gzip compressed data, was "zern-0.0.2.tar", last modified: Thu May  2 18:46:04 2024, max compression
```

## Comparing `zern-0.0.1.tar` & `zern-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,23 @@
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 17:58:39.575047 zern-0.0.1/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     1071 2024-05-02 15:26:31.000000 zern-0.0.1/LICENSE
--rw-r--r--   0 harsha    (1000) harsha    (1000)     6341 2024-05-02 17:58:39.575047 zern-0.0.1/PKG-INFO
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     5716 2024-05-02 15:26:53.000000 zern-0.0.1/README.md
--rw-rw-r--   0 harsha    (1000) harsha    (1000)      623 2024-05-02 17:53:39.000000 zern-0.0.1/pyproject.toml
--rw-rw-r--   0 harsha    (1000) harsha    (1000)       38 2024-05-02 17:58:39.575047 zern-0.0.1/setup.cfg
--rw-rw-r--   0 harsha    (1000) harsha    (1000)      613 2024-05-02 15:41:26.000000 zern-0.0.1/setup.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 17:58:39.575047 zern-0.0.1/zern.egg-info/
--rw-r--r--   0 harsha    (1000) harsha    (1000)     6341 2024-05-02 17:58:39.000000 zern-0.0.1/zern.egg-info/PKG-INFO
--rw-rw-r--   0 harsha    (1000) harsha    (1000)      153 2024-05-02 17:58:39.000000 zern-0.0.1/zern.egg-info/SOURCES.txt
--rw-rw-r--   0 harsha    (1000) harsha    (1000)        1 2024-05-02 17:58:39.000000 zern-0.0.1/zern.egg-info/dependency_links.txt
--rw-rw-r--   0 harsha    (1000) harsha    (1000)        1 2024-05-02 17:58:39.000000 zern-0.0.1/zern.egg-info/top_level.txt
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 18:46:04.228110 zern-0.0.2/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     1071 2024-05-02 15:26:31.000000 zern-0.0.2/LICENSE
+-rw-r--r--   0 harsha    (1000) harsha    (1000)     6270 2024-05-02 18:46:04.228110 zern-0.0.2/PKG-INFO
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     5716 2024-05-02 15:26:53.000000 zern-0.0.2/README.md
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)      623 2024-05-02 18:45:17.000000 zern-0.0.2/pyproject.toml
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)       38 2024-05-02 18:46:04.228110 zern-0.0.2/setup.cfg
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 18:46:04.224110 zern-0.0.2/src/
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 18:46:04.224110 zern-0.0.2/src/zern/
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 18:46:04.228110 zern-0.0.2/src/zern/Core/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     3798 2024-05-02 06:23:51.000000 zern-0.0.2/src/zern/Core/session.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     4638 2024-05-02 06:32:36.000000 zern-0.0.2/src/zern/Core/trader.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 18:46:04.228110 zern-0.0.2/src/zern/Core/websocket/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     3534 2024-05-02 07:34:58.000000 zern-0.0.2/src/zern/Core/websocket/ticker.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)       61 2024-04-24 18:27:30.000000 zern-0.0.2/src/zern/__init__.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 18:46:04.228110 zern-0.0.2/src/zern/utils/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     1861 2024-04-21 19:33:12.000000 zern-0.0.2/src/zern/utils/OrderedList.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     2280 2024-05-02 05:29:49.000000 zern-0.0.2/src/zern/utils/Types.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     6314 2024-05-02 05:36:04.000000 zern-0.0.2/src/zern/utils/parsing.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 18:46:04.228110 zern-0.0.2/src/zern.egg-info/
+-rw-r--r--   0 harsha    (1000) harsha    (1000)     6270 2024-05-02 18:46:04.000000 zern-0.0.2/src/zern.egg-info/PKG-INFO
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)      344 2024-05-02 18:46:04.000000 zern-0.0.2/src/zern.egg-info/SOURCES.txt
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)        1 2024-05-02 18:46:04.000000 zern-0.0.2/src/zern.egg-info/dependency_links.txt
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)        5 2024-05-02 18:46:04.000000 zern-0.0.2/src/zern.egg-info/top_level.txt
```

### Comparing `zern-0.0.1/LICENSE` & `zern-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zern-0.0.1/PKG-INFO` & `zern-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: zern
-Version: 0.0.1
+Version: 0.0.2
 Summary: An unofficial client library using Zerodha web api for live data and historical data
-Home-page: https://github.com/ExBlacklight/Zern
-Author: Harsha Avapati
 Author-email: Harsha Avapati <harshaavapati@gmail.com>
 Project-URL: Homepage, https://github.com/ExBlacklight/Zern
 Project-URL: Issues, https://github.com/ExBlacklight/Zern/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `zern-0.0.1/README.md` & `zern-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `zern-0.0.1/pyproject.toml` & `zern-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zern"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Harsha Avapati", email="harshaavapati@gmail.com" },
 ]
 description = "An unofficial client library using Zerodha web api for live data and historical data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `zern-0.0.1/zern.egg-info/PKG-INFO` & `zern-0.0.2/src/zern.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: zern
-Version: 0.0.1
+Version: 0.0.2
 Summary: An unofficial client library using Zerodha web api for live data and historical data
-Home-page: https://github.com/ExBlacklight/Zern
-Author: Harsha Avapati
 Author-email: Harsha Avapati <harshaavapati@gmail.com>
 Project-URL: Homepage, https://github.com/ExBlacklight/Zern
 Project-URL: Issues, https://github.com/ExBlacklight/Zern/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

