# Comparing `tmp/apmtools-0.0.8.tar.gz` & `tmp/apmtools-0.0.9.tar.gz`

## Comparing `apmtools-0.0.8.tar` & `apmtools-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0  4949333 2020-02-02 00:00:00.000000 apmtools-0.0.8/test.zip
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apmtools-0.0.8/src/apmtools/__init__.py
--rw-r--r--   0        0        0    10420 2020-02-02 00:00:00.000000 apmtools-0.0.8/src/apmtools/classes.py
--rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 apmtools-0.0.8/src/apmtools/data_processing.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 apmtools-0.0.8/src/apmtools/functions.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 apmtools-0.0.8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 apmtools-0.0.8/LICENSE
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 apmtools-0.0.8/README.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 apmtools-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 apmtools-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0  4949333 2020-02-02 00:00:00.000000 apmtools-0.0.9/test.zip
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apmtools-0.0.9/src/apmtools/__init__.py
+-rw-r--r--   0        0        0    10424 2020-02-02 00:00:00.000000 apmtools-0.0.9/src/apmtools/classes.py
+-rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 apmtools-0.0.9/src/apmtools/data_processing.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 apmtools-0.0.9/src/apmtools/functions.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 apmtools-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 apmtools-0.0.9/LICENSE
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 apmtools-0.0.9/README.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 apmtools-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 apmtools-0.0.9/PKG-INFO
```

### Comparing `apmtools-0.0.8/test.zip` & `apmtools-0.0.9/test.zip`

 * *Files identical despite different names*

### Comparing `apmtools-0.0.8/src/apmtools/classes.py` & `apmtools-0.0.9/src/apmtools/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                         try:
                             if value.__getattr__(i) not in j:
                                 del a[key]
                         except:
                             pass
 
         return DictionaryPlus(a)
-
+    
 
     def set_attrib(self, attribute):
         """
         returns the set of attribute values for dictionary
         """
         return_set = set()
         for i in self.values():
```

### Comparing `apmtools-0.0.8/src/apmtools/data_processing.py` & `apmtools-0.0.9/src/apmtools/data_processing.py`

 * *Files identical despite different names*

### Comparing `apmtools-0.0.8/LICENSE` & `apmtools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `apmtools-0.0.8/pyproject.toml` & `apmtools-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "apmtools"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Federico Lorenzetti", email="lorenzetti.federico@gmail.com" },
 ]
 description = "A collection of tools for processing air pollution monitoring data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `apmtools-0.0.8/PKG-INFO` & `apmtools-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: apmtools
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of tools for processing air pollution monitoring data
 Project-URL: Homepage, https://github.com/federlorenz/apmtools
 Author-email: Federico Lorenzetti <lorenzetti.federico@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

