# Comparing `tmp/pyfujitsugeneral-2.0.8.tar.gz` & `tmp/pyfujitsugeneral-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfujitsugeneral-2.0.8.tar", last modified: Thu Nov 16 17:59:58 2023, max compression
+gzip compressed data, was "pyfujitsugeneral-2.0.9.tar", last modified: Thu Nov 16 18:25:00 2023, max compression
```

## Comparing `pyfujitsugeneral-2.0.8.tar` & `pyfujitsugeneral-2.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 bigmoby    (501) staff       (20)        0 2023-11-16 17:59:58.783985 pyfujitsugeneral-2.0.8/
--rw-r--r--   0 bigmoby    (501) staff       (20)     1102 2023-03-01 12:48:11.000000 pyfujitsugeneral-2.0.8/LICENSE
--rw-r--r--   0 bigmoby    (501) staff       (20)      789 2023-11-16 17:59:58.783559 pyfujitsugeneral-2.0.8/PKG-INFO
--rw-r--r--   0 bigmoby    (501) staff       (20)       98 2023-03-01 15:50:34.000000 pyfujitsugeneral-2.0.8/README.md
-drwxr-xr-x   0 bigmoby    (501) staff       (20)        0 2023-11-16 17:59:58.774302 pyfujitsugeneral-2.0.8/pyfujitsugeneral/
--rw-r--r--   0 bigmoby    (501) staff       (20)      111 2023-03-01 15:43:25.000000 pyfujitsugeneral-2.0.8/pyfujitsugeneral/__init__.py
--rw-r--r--   0 bigmoby    (501) staff       (20)     8950 2023-11-16 17:50:52.000000 pyfujitsugeneral-2.0.8/pyfujitsugeneral/client.py
--rw-r--r--   0 bigmoby    (501) staff       (20)      964 2023-10-13 17:49:35.000000 pyfujitsugeneral-2.0.8/pyfujitsugeneral/exceptions.py
--rw-r--r--   0 bigmoby    (501) staff       (20)    24608 2023-11-16 17:54:12.000000 pyfujitsugeneral-2.0.8/pyfujitsugeneral/splitac.py
--rw-r--r--   0 bigmoby    (501) staff       (20)      260 2023-10-13 17:49:56.000000 pyfujitsugeneral-2.0.8/pyfujitsugeneral/utils.py
-drwxr-xr-x   0 bigmoby    (501) staff       (20)        0 2023-11-16 17:59:58.782279 pyfujitsugeneral-2.0.8/pyfujitsugeneral.egg-info/
--rw-r--r--   0 bigmoby    (501) staff       (20)      789 2023-11-16 17:59:58.000000 pyfujitsugeneral-2.0.8/pyfujitsugeneral.egg-info/PKG-INFO
--rw-r--r--   0 bigmoby    (501) staff       (20)      376 2023-11-16 17:59:58.000000 pyfujitsugeneral-2.0.8/pyfujitsugeneral.egg-info/SOURCES.txt
--rw-r--r--   0 bigmoby    (501) staff       (20)        1 2023-11-16 17:59:58.000000 pyfujitsugeneral-2.0.8/pyfujitsugeneral.egg-info/dependency_links.txt
--rw-r--r--   0 bigmoby    (501) staff       (20)       44 2023-11-16 17:59:58.000000 pyfujitsugeneral-2.0.8/pyfujitsugeneral.egg-info/requires.txt
--rw-r--r--   0 bigmoby    (501) staff       (20)       17 2023-11-16 17:59:58.000000 pyfujitsugeneral-2.0.8/pyfujitsugeneral.egg-info/top_level.txt
--rw-r--r--   0 bigmoby    (501) staff       (20)       79 2023-11-16 17:59:58.785774 pyfujitsugeneral-2.0.8/setup.cfg
--rw-r--r--   0 bigmoby    (501) staff       (20)      964 2023-11-16 17:53:41.000000 pyfujitsugeneral-2.0.8/setup.py
+drwxr-xr-x   0 bigmoby    (501) staff       (20)        0 2023-11-16 18:25:00.560220 pyfujitsugeneral-2.0.9/
+-rw-r--r--   0 bigmoby    (501) staff       (20)     1102 2023-03-01 12:48:11.000000 pyfujitsugeneral-2.0.9/LICENSE
+-rw-r--r--   0 bigmoby    (501) staff       (20)      789 2023-11-16 18:25:00.559904 pyfujitsugeneral-2.0.9/PKG-INFO
+-rw-r--r--   0 bigmoby    (501) staff       (20)       98 2023-03-01 15:50:34.000000 pyfujitsugeneral-2.0.9/README.md
+drwxr-xr-x   0 bigmoby    (501) staff       (20)        0 2023-11-16 18:25:00.547354 pyfujitsugeneral-2.0.9/pyfujitsugeneral/
+-rw-r--r--   0 bigmoby    (501) staff       (20)      111 2023-03-01 15:43:25.000000 pyfujitsugeneral-2.0.9/pyfujitsugeneral/__init__.py
+-rw-r--r--   0 bigmoby    (501) staff       (20)     8950 2023-11-16 18:20:34.000000 pyfujitsugeneral-2.0.9/pyfujitsugeneral/client.py
+-rw-r--r--   0 bigmoby    (501) staff       (20)      964 2023-10-13 17:49:35.000000 pyfujitsugeneral-2.0.9/pyfujitsugeneral/exceptions.py
+-rw-r--r--   0 bigmoby    (501) staff       (20)    24894 2023-11-16 18:21:27.000000 pyfujitsugeneral-2.0.9/pyfujitsugeneral/splitac.py
+-rw-r--r--   0 bigmoby    (501) staff       (20)      260 2023-10-13 17:49:56.000000 pyfujitsugeneral-2.0.9/pyfujitsugeneral/utils.py
+drwxr-xr-x   0 bigmoby    (501) staff       (20)        0 2023-11-16 18:25:00.558662 pyfujitsugeneral-2.0.9/pyfujitsugeneral.egg-info/
+-rw-r--r--   0 bigmoby    (501) staff       (20)      789 2023-11-16 18:25:00.000000 pyfujitsugeneral-2.0.9/pyfujitsugeneral.egg-info/PKG-INFO
+-rw-r--r--   0 bigmoby    (501) staff       (20)      376 2023-11-16 18:25:00.000000 pyfujitsugeneral-2.0.9/pyfujitsugeneral.egg-info/SOURCES.txt
+-rw-r--r--   0 bigmoby    (501) staff       (20)        1 2023-11-16 18:25:00.000000 pyfujitsugeneral-2.0.9/pyfujitsugeneral.egg-info/dependency_links.txt
+-rw-r--r--   0 bigmoby    (501) staff       (20)       44 2023-11-16 18:25:00.000000 pyfujitsugeneral-2.0.9/pyfujitsugeneral.egg-info/requires.txt
+-rw-r--r--   0 bigmoby    (501) staff       (20)       17 2023-11-16 18:25:00.000000 pyfujitsugeneral-2.0.9/pyfujitsugeneral.egg-info/top_level.txt
+-rw-r--r--   0 bigmoby    (501) staff       (20)       79 2023-11-16 18:25:00.561938 pyfujitsugeneral-2.0.9/setup.cfg
+-rw-r--r--   0 bigmoby    (501) staff       (20)      964 2023-11-16 18:11:54.000000 pyfujitsugeneral-2.0.9/setup.py
```

### Comparing `pyfujitsugeneral-2.0.8/LICENSE` & `pyfujitsugeneral-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfujitsugeneral-2.0.8/PKG-INFO` & `pyfujitsugeneral-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfujitsugeneral
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python Library for interacting with Fujitsu General split air conditioners API
 Home-page: https://github.com/bigmoby/pyfujitsugeneral
 Download-URL: https://github.com/bigmoby/pyfujitsugeneral
 Author: Fabio Mauro, Mehdi Modarressi
 Author-email: bigmoby.pymeianlike@gmail.com
 License: MIT License
 Keywords: Fujitsu General air conditioners
```

### Comparing `pyfujitsugeneral-2.0.8/pyfujitsugeneral/client.py` & `pyfujitsugeneral-2.0.9/pyfujitsugeneral/client.py`

 * *Files identical despite different names*

### Comparing `pyfujitsugeneral-2.0.8/pyfujitsugeneral/exceptions.py` & `pyfujitsugeneral-2.0.9/pyfujitsugeneral/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyfujitsugeneral-2.0.8/pyfujitsugeneral/splitac.py` & `pyfujitsugeneral-2.0.9/pyfujitsugeneral/splitac.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,27 @@
 from .exceptions import FGLairMethodException, FGLairGeneralException
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def get_prop_from_json(property_name: str, properties: Any) -> dict[str, Any]:
-    data = {}
     for property_item in properties:
         if property_item["property"]["name"] == property_name:
-            data = {
+            if property_name == "refresh":
+                return {
+                    "value": property_item["property"]["value"],
+                    "key": property_item["property"]["key"],
+                    "data_updated_at": property_item["property"]["data_updated_at"],
+                }
+            return {
                 "value": property_item["property"]["value"],
                 "key": property_item["property"]["key"],
             }
-    return data
+    return {}
 
 
 class SplitAC:
     def __init__(
         self,
         dsn: str,
         client: FGLairApiClient,
```

### Comparing `pyfujitsugeneral-2.0.8/pyfujitsugeneral.egg-info/PKG-INFO` & `pyfujitsugeneral-2.0.9/pyfujitsugeneral.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfujitsugeneral
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python Library for interacting with Fujitsu General split air conditioners API
 Home-page: https://github.com/bigmoby/pyfujitsugeneral
 Download-URL: https://github.com/bigmoby/pyfujitsugeneral
 Author: Fabio Mauro, Mehdi Modarressi
 Author-email: bigmoby.pymeianlike@gmail.com
 License: MIT License
 Keywords: Fujitsu General air conditioners
```

### Comparing `pyfujitsugeneral-2.0.8/setup.py` & `pyfujitsugeneral-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 setup(
     name="pyfujitsugeneral",
     py_modules=["pyfujitsugeneral"],
     version=__version__,
     description="Python Library for interacting with Fujitsu General split air conditioners API",
     long_description="Python Library for interacting with Fujitsu General split air conditioners API",
```

