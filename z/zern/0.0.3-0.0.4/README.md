# Comparing `tmp/zern-0.0.3.tar.gz` & `tmp/zern-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zern-0.0.3.tar", last modified: Thu May  2 19:29:41 2024, max compression
+gzip compressed data, was "zern-0.0.4.tar", last modified: Thu May  2 19:48:22 2024, max compression
```

## Comparing `zern-0.0.3.tar` & `zern-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:29:41.785089 zern-0.0.3/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     1071 2024-05-02 15:26:31.000000 zern-0.0.3/LICENSE
--rw-r--r--   0 harsha    (1000) harsha    (1000)     6270 2024-05-02 19:29:41.785089 zern-0.0.3/PKG-INFO
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     5716 2024-05-02 15:26:53.000000 zern-0.0.3/README.md
--rw-rw-r--   0 harsha    (1000) harsha    (1000)      707 2024-05-02 19:11:35.000000 zern-0.0.3/pyproject.toml
--rw-rw-r--   0 harsha    (1000) harsha    (1000)       38 2024-05-02 19:29:41.785089 zern-0.0.3/setup.cfg
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:29:41.785089 zern-0.0.3/src/
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:29:41.785089 zern-0.0.3/src/zern/
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:29:41.785089 zern-0.0.3/src/zern/Core/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     3798 2024-05-02 06:23:51.000000 zern-0.0.3/src/zern/Core/session.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     4646 2024-05-02 19:27:04.000000 zern-0.0.3/src/zern/Core/trader.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:29:41.785089 zern-0.0.3/src/zern/Core/websocket_connection/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     3534 2024-05-02 07:34:58.000000 zern-0.0.3/src/zern/Core/websocket_connection/ticker.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)       61 2024-04-24 18:27:30.000000 zern-0.0.3/src/zern/__init__.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:29:41.785089 zern-0.0.3/src/zern/utils/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     1861 2024-04-21 19:33:12.000000 zern-0.0.3/src/zern/utils/OrderedList.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     2280 2024-05-02 05:29:49.000000 zern-0.0.3/src/zern/utils/Types.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     6314 2024-05-02 05:36:04.000000 zern-0.0.3/src/zern/utils/parsing.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:29:41.785089 zern-0.0.3/src/zern.egg-info/
--rw-r--r--   0 harsha    (1000) harsha    (1000)     6270 2024-05-02 19:29:41.000000 zern-0.0.3/src/zern.egg-info/PKG-INFO
--rw-rw-r--   0 harsha    (1000) harsha    (1000)      355 2024-05-02 19:29:41.000000 zern-0.0.3/src/zern.egg-info/SOURCES.txt
--rw-rw-r--   0 harsha    (1000) harsha    (1000)        1 2024-05-02 19:29:41.000000 zern-0.0.3/src/zern.egg-info/dependency_links.txt
--rw-rw-r--   0 harsha    (1000) harsha    (1000)        5 2024-05-02 19:29:41.000000 zern-0.0.3/src/zern.egg-info/top_level.txt
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:48:22.257508 zern-0.0.4/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     1071 2024-05-02 15:26:31.000000 zern-0.0.4/LICENSE
+-rw-r--r--   0 harsha    (1000) harsha    (1000)     6270 2024-05-02 19:48:22.257508 zern-0.0.4/PKG-INFO
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     5716 2024-05-02 15:26:53.000000 zern-0.0.4/README.md
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)      767 2024-05-02 19:48:16.000000 zern-0.0.4/pyproject.toml
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)       38 2024-05-02 19:48:22.257508 zern-0.0.4/setup.cfg
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:48:22.253508 zern-0.0.4/src/
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:48:22.253508 zern-0.0.4/src/zern/
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:48:22.253508 zern-0.0.4/src/zern/Core/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     3798 2024-05-02 06:23:51.000000 zern-0.0.4/src/zern/Core/session.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     4646 2024-05-02 19:27:04.000000 zern-0.0.4/src/zern/Core/trader.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:48:22.253508 zern-0.0.4/src/zern/Core/websocket_connection/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     3534 2024-05-02 07:34:58.000000 zern-0.0.4/src/zern/Core/websocket_connection/ticker.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)       61 2024-04-24 18:27:30.000000 zern-0.0.4/src/zern/__init__.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:48:22.253508 zern-0.0.4/src/zern/utils/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     1861 2024-04-21 19:33:12.000000 zern-0.0.4/src/zern/utils/OrderedList.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     2280 2024-05-02 05:29:49.000000 zern-0.0.4/src/zern/utils/Types.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     6314 2024-05-02 05:36:04.000000 zern-0.0.4/src/zern/utils/parsing.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:48:22.253508 zern-0.0.4/src/zern.egg-info/
+-rw-r--r--   0 harsha    (1000) harsha    (1000)     6270 2024-05-02 19:48:22.000000 zern-0.0.4/src/zern.egg-info/PKG-INFO
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)      355 2024-05-02 19:48:22.000000 zern-0.0.4/src/zern.egg-info/SOURCES.txt
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)        1 2024-05-02 19:48:22.000000 zern-0.0.4/src/zern.egg-info/dependency_links.txt
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)        5 2024-05-02 19:48:22.000000 zern-0.0.4/src/zern.egg-info/top_level.txt
```

### Comparing `zern-0.0.3/LICENSE` & `zern-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zern-0.0.3/PKG-INFO` & `zern-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zern
-Version: 0.0.3
+Version: 0.0.4
 Summary: An unofficial client library using Zerodha web api for live data and historical data
 Author-email: Harsha Avapati <harshaavapati@gmail.com>
 Project-URL: Homepage, https://github.com/ExBlacklight/Zern
 Project-URL: Issues, https://github.com/ExBlacklight/Zern/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `zern-0.0.3/README.md` & `zern-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `zern-0.0.3/pyproject.toml` & `zern-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=61.0","websocket-client<=1.8.0","pyotp<=2.9.0","requests<=2.31.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zern"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Harsha Avapati", email="harshaavapati@gmail.com" },
 ]
 description = "An unofficial client library using Zerodha web api for live data and historical data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `zern-0.0.3/src/zern/Core/session.py` & `zern-0.0.4/src/zern/Core/session.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.3/src/zern/Core/trader.py` & `zern-0.0.4/src/zern/Core/trader.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.3/src/zern/Core/websocket_connection/ticker.py` & `zern-0.0.4/src/zern/Core/websocket_connection/ticker.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.3/src/zern/utils/OrderedList.py` & `zern-0.0.4/src/zern/utils/OrderedList.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.3/src/zern/utils/Types.py` & `zern-0.0.4/src/zern/utils/Types.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.3/src/zern/utils/parsing.py` & `zern-0.0.4/src/zern/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.3/src/zern.egg-info/PKG-INFO` & `zern-0.0.4/src/zern.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zern
-Version: 0.0.3
+Version: 0.0.4
 Summary: An unofficial client library using Zerodha web api for live data and historical data
 Author-email: Harsha Avapati <harshaavapati@gmail.com>
 Project-URL: Homepage, https://github.com/ExBlacklight/Zern
 Project-URL: Issues, https://github.com/ExBlacklight/Zern/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

