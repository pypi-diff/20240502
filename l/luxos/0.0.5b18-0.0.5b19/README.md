# Comparing `tmp/luxos-0.0.5b18.tar.gz` & `tmp/luxos-0.0.5b19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luxos-0.0.5b18.tar", last modified: Tue Apr 30 18:47:03 2024, max compression
+gzip compressed data, was "luxos-0.0.5b19.tar", last modified: Thu May  2 15:00:06 2024, max compression
```

## Comparing `luxos-0.0.5b18.tar` & `luxos-0.0.5b19.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:47:03.709884 luxos-0.0.5b18/
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-30 18:47:03.709884 luxos-0.0.5b18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-30 18:46:32.000000 luxos-0.0.5b18/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-30 18:47:01.000000 luxos-0.0.5b18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 18:47:03.709884 luxos-0.0.5b18/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:47:03.705884 luxos-0.0.5b18/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:47:03.709884 luxos-0.0.5b18/src/luxos/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-30 18:47:01.000000 luxos-0.0.5b18/src/luxos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 18:46:32.000000 luxos-0.0.5b18/src/luxos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-30 18:46:32.000000 luxos-0.0.5b18/src/luxos/api.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-30 18:46:32.000000 luxos-0.0.5b18/src/luxos/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-04-30 18:46:32.000000 luxos-0.0.5b18/src/luxos/asyncops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:47:03.709884 luxos-0.0.5b18/src/luxos/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:46:32.000000 luxos-0.0.5b18/src/luxos/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-30 18:46:32.000000 luxos-0.0.5b18/src/luxos/cli/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 18:46:32.000000 luxos-0.0.5b18/src/luxos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-30 18:46:32.000000 luxos-0.0.5b18/src/luxos/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:46:32.000000 luxos-0.0.5b18/src/luxos/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:47:03.709884 luxos-0.0.5b18/src/luxos/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:46:32.000000 luxos-0.0.5b18/src/luxos/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-30 18:46:32.000000 luxos-0.0.5b18/src/luxos/scripts/async_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-04-30 18:46:32.000000 luxos-0.0.5b18/src/luxos/scripts/health_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-30 18:46:32.000000 luxos-0.0.5b18/src/luxos/scripts/luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-30 18:46:32.000000 luxos-0.0.5b18/src/luxos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:47:03.709884 luxos-0.0.5b18/src/luxos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-30 18:47:03.000000 luxos-0.0.5b18/src/luxos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-30 18:47:03.000000 luxos-0.0.5b18/src/luxos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:47:03.000000 luxos-0.0.5b18/src/luxos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-30 18:47:03.000000 luxos-0.0.5b18/src/luxos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-30 18:47:03.000000 luxos-0.0.5b18/src/luxos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 18:47:03.000000 luxos-0.0.5b18/src/luxos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:47:03.709884 luxos-0.0.5b18/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-30 18:46:32.000000 luxos-0.0.5b18/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-30 18:46:32.000000 luxos-0.0.5b18/tests/test_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-04-30 18:46:32.000000 luxos-0.0.5b18/tests/test_luxos_asyncops.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-30 18:46:32.000000 luxos-0.0.5b18/tests/test_luxos_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:00:06.916602 luxos-0.0.5b19/
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-02 15:00:06.916602 luxos-0.0.5b19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-02 14:59:37.000000 luxos-0.0.5b19/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-02 15:00:04.000000 luxos-0.0.5b19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:00:06.916602 luxos-0.0.5b19/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:00:06.912603 luxos-0.0.5b19/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:00:06.916602 luxos-0.0.5b19/src/luxos/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-02 15:00:04.000000 luxos-0.0.5b19/src/luxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-02 14:59:37.000000 luxos-0.0.5b19/src/luxos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-02 14:59:37.000000 luxos-0.0.5b19/src/luxos/api.json
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-02 14:59:37.000000 luxos-0.0.5b19/src/luxos/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-02 14:59:37.000000 luxos-0.0.5b19/src/luxos/asyncops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:00:06.916602 luxos-0.0.5b19/src/luxos/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:59:37.000000 luxos-0.0.5b19/src/luxos/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-02 14:59:37.000000 luxos-0.0.5b19/src/luxos/cli/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-02 14:59:37.000000 luxos-0.0.5b19/src/luxos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-02 14:59:37.000000 luxos-0.0.5b19/src/luxos/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:59:37.000000 luxos-0.0.5b19/src/luxos/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:00:06.916602 luxos-0.0.5b19/src/luxos/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:59:37.000000 luxos-0.0.5b19/src/luxos/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-02 14:59:37.000000 luxos-0.0.5b19/src/luxos/scripts/async_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-05-02 14:59:37.000000 luxos-0.0.5b19/src/luxos/scripts/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-02 14:59:37.000000 luxos-0.0.5b19/src/luxos/scripts/luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-02 14:59:37.000000 luxos-0.0.5b19/src/luxos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:00:06.916602 luxos-0.0.5b19/src/luxos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-02 15:00:06.000000 luxos-0.0.5b19/src/luxos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-02 15:00:06.000000 luxos-0.0.5b19/src/luxos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:00:06.000000 luxos-0.0.5b19/src/luxos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-02 15:00:06.000000 luxos-0.0.5b19/src/luxos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 15:00:06.000000 luxos-0.0.5b19/src/luxos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 15:00:06.000000 luxos-0.0.5b19/src/luxos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:00:06.916602 luxos-0.0.5b19/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-02 14:59:37.000000 luxos-0.0.5b19/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-02 14:59:37.000000 luxos-0.0.5b19/tests/test_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-02 14:59:37.000000 luxos-0.0.5b19/tests/test_luxos_asyncops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-02 14:59:37.000000 luxos-0.0.5b19/tests/test_luxos_misc.py
```

### Comparing `luxos-0.0.5b18/PKG-INFO` & `luxos-0.0.5b19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.5b18
+Version: 0.0.5b19
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.5b18/README.md` & `luxos-0.0.5b19/README.md`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b18/pyproject.toml` & `luxos-0.0.5b19/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "luxos"
-version = "0.0.5b18"
+version = "0.0.5b19"
 description = "The all encompassing LuxOS python library."
 readme = "README.md"
 license = { text = "MIT" }  # TODO I don't think this is a MIT??
 requires-python = ">= 3.9"
 
 authors = [
   { name = "Antonio Cavallo", email = "antonio.cavallo@luxor.tech" },
```

### Comparing `luxos-0.0.5b18/src/luxos/api.json` & `luxos-0.0.5b19/src/luxos/api.json`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b18/src/luxos/api.py` & `luxos-0.0.5b19/src/luxos/api.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b18/src/luxos/asyncops.py` & `luxos-0.0.5b19/src/luxos/asyncops.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b18/src/luxos/cli/v1.py` & `luxos-0.0.5b19/src/luxos/cli/v1.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b18/src/luxos/exceptions.py` & `luxos-0.0.5b19/src/luxos/exceptions.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b18/src/luxos/misc.py` & `luxos-0.0.5b19/src/luxos/misc.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b18/src/luxos/scripts/async_luxos.py` & `luxos-0.0.5b19/src/luxos/scripts/async_luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b18/src/luxos/scripts/health_checker.py` & `luxos-0.0.5b19/src/luxos/scripts/health_checker.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b18/src/luxos/scripts/luxos.py` & `luxos-0.0.5b19/src/luxos/scripts/luxos.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,14 +371,14 @@
             threads = []
 
     # Wait for the remaining threads to finish
     for thread in threads:
         thread.join()
 
     # Execution completed
-    end_time = time.time()
+    end_time = time.monotonic()
     execution_time = end_time - start_time
     log.info(f"Execution completed in {execution_time:.2f} seconds.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `luxos-0.0.5b18/src/luxos/utils.py` & `luxos-0.0.5b19/src/luxos/utils.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b18/src/luxos.egg-info/PKG-INFO` & `luxos-0.0.5b19/src/luxos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.5b18
+Version: 0.0.5b19
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.5b18/src/luxos.egg-info/SOURCES.txt` & `luxos-0.0.5b19/src/luxos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b18/tests/test_cli.py` & `luxos-0.0.5b19/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b18/tests/test_luxos_asyncops.py` & `luxos-0.0.5b19/tests/test_luxos_asyncops.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b18/tests/test_luxos_misc.py` & `luxos-0.0.5b19/tests/test_luxos_misc.py`

 * *Files identical despite different names*

