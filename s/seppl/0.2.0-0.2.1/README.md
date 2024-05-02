# Comparing `tmp/seppl-0.2.0.tar.gz` & `tmp/seppl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seppl-0.2.0.tar", last modified: Wed May  1 03:41:31 2024, max compression
+gzip compressed data, was "seppl-0.2.1.tar", last modified: Thu May  2 01:25:40 2024, max compression
```

## Comparing `seppl-0.2.0.tar` & `seppl-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-01 03:41:31.413744 seppl-0.2.0/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4060 2024-05-01 03:40:48.000000 seppl-0.2.0/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      568 2023-11-09 01:56:09.000000 seppl-0.2.0/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 seppl-0.2.0/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6253 2024-05-01 03:41:31.413744 seppl-0.2.0/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3741 2024-05-01 03:08:55.000000 seppl-0.2.0/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2024-05-01 03:41:31.413744 seppl-0.2.0/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1130 2024-05-01 03:40:48.000000 seppl-0.2.0/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-01 03:41:31.409744 seppl-0.2.0/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-01 03:41:31.413744 seppl-0.2.0/src/seppl/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      765 2024-04-30 23:53:36.000000 seppl-0.2.0/src/seppl/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5702 2024-02-21 21:20:08.000000 seppl-0.2.0/src/seppl/_args.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    16420 2024-05-01 01:31:12.000000 seppl-0.2.0/src/seppl/_class_registry.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1719 2023-10-04 19:59:54.000000 seppl-0.2.0/src/seppl/_entry_points.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2876 2023-10-04 20:28:17.000000 seppl-0.2.0/src/seppl/_help.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1942 2024-02-04 21:21:35.000000 seppl-0.2.0/src/seppl/_metadata.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8347 2024-02-28 19:32:25.000000 seppl-0.2.0/src/seppl/_plugin.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    15743 2024-04-30 23:41:51.000000 seppl-0.2.0/src/seppl/_registry.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1679 2024-02-04 21:33:05.000000 seppl-0.2.0/src/seppl/_session.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2623 2024-02-28 19:32:25.000000 seppl-0.2.0/src/seppl/_types.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-01 03:41:31.413744 seppl-0.2.0/src/seppl/io/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      282 2024-02-05 00:23:10.000000 seppl-0.2.0/src/seppl/io/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5553 2024-03-21 01:02:31.000000 seppl-0.2.0/src/seppl/io/_execution.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6560 2024-02-04 23:34:50.000000 seppl-0.2.0/src/seppl/io/_filter.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1555 2024-02-04 23:40:54.000000 seppl-0.2.0/src/seppl/io/_reader.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3147 2024-02-07 03:48:04.000000 seppl-0.2.0/src/seppl/io/_split.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2444 2024-02-05 00:23:10.000000 seppl-0.2.0/src/seppl/io/_utils.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3319 2024-02-04 23:40:54.000000 seppl-0.2.0/src/seppl/io/_writer.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-01 03:41:31.413744 seppl-0.2.0/src/seppl/tool/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2024-02-21 20:25:44.000000 seppl-0.2.0/src/seppl/tool/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      772 2024-02-21 20:32:02.000000 seppl-0.2.0/src/seppl/tool/escape.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      780 2024-02-21 20:32:02.000000 seppl-0.2.0/src/seppl/tool/unescape.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-01 03:41:31.413744 seppl-0.2.0/src/seppl.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6253 2024-05-01 03:41:31.000000 seppl-0.2.0/src/seppl.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      700 2024-05-01 03:41:31.000000 seppl-0.2.0/src/seppl.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2024-05-01 03:41:31.000000 seppl-0.2.0/src/seppl.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      107 2024-05-01 03:41:31.000000 seppl-0.2.0/src/seppl.egg-info/entry_points.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        6 2024-05-01 03:41:31.000000 seppl-0.2.0/src/seppl.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 01:25:40.571310 seppl-0.2.1/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4192 2024-05-02 01:22:58.000000 seppl-0.2.1/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      568 2023-11-09 01:56:09.000000 seppl-0.2.1/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 seppl-0.2.1/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6433 2024-05-02 01:25:40.571310 seppl-0.2.1/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3741 2024-05-01 21:38:44.000000 seppl-0.2.1/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2024-05-02 01:25:40.571310 seppl-0.2.1/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1130 2024-05-02 01:22:58.000000 seppl-0.2.1/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 01:25:40.567310 seppl-0.2.1/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 01:25:40.571310 seppl-0.2.1/src/seppl/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      765 2024-04-30 23:53:36.000000 seppl-0.2.1/src/seppl/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5702 2024-02-21 21:20:08.000000 seppl-0.2.1/src/seppl/_args.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    16546 2024-05-02 01:21:14.000000 seppl-0.2.1/src/seppl/_class_registry.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1719 2023-10-04 19:59:54.000000 seppl-0.2.1/src/seppl/_entry_points.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2876 2023-10-04 20:28:17.000000 seppl-0.2.1/src/seppl/_help.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1942 2024-02-04 21:21:35.000000 seppl-0.2.1/src/seppl/_metadata.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8347 2024-02-28 19:32:25.000000 seppl-0.2.1/src/seppl/_plugin.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    15743 2024-04-30 23:41:51.000000 seppl-0.2.1/src/seppl/_registry.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1679 2024-02-04 21:33:05.000000 seppl-0.2.1/src/seppl/_session.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2623 2024-02-28 19:32:25.000000 seppl-0.2.1/src/seppl/_types.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 01:25:40.571310 seppl-0.2.1/src/seppl/io/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      282 2024-02-05 00:23:10.000000 seppl-0.2.1/src/seppl/io/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5553 2024-03-21 01:02:31.000000 seppl-0.2.1/src/seppl/io/_execution.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6560 2024-02-04 23:34:50.000000 seppl-0.2.1/src/seppl/io/_filter.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1555 2024-02-04 23:40:54.000000 seppl-0.2.1/src/seppl/io/_reader.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3147 2024-02-07 03:48:04.000000 seppl-0.2.1/src/seppl/io/_split.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2444 2024-02-05 00:23:10.000000 seppl-0.2.1/src/seppl/io/_utils.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3319 2024-02-04 23:40:54.000000 seppl-0.2.1/src/seppl/io/_writer.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 01:25:40.571310 seppl-0.2.1/src/seppl/tool/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2024-02-21 20:25:44.000000 seppl-0.2.1/src/seppl/tool/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      772 2024-02-21 20:32:02.000000 seppl-0.2.1/src/seppl/tool/escape.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      780 2024-02-21 20:32:02.000000 seppl-0.2.1/src/seppl/tool/unescape.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 01:25:40.571310 seppl-0.2.1/src/seppl.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6433 2024-05-02 01:25:40.000000 seppl-0.2.1/src/seppl.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      700 2024-05-02 01:25:40.000000 seppl-0.2.1/src/seppl.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2024-05-02 01:25:40.000000 seppl-0.2.1/src/seppl.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      107 2024-05-02 01:25:40.000000 seppl-0.2.1/src/seppl.egg-info/entry_points.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        6 2024-05-02 01:25:40.000000 seppl-0.2.1/src/seppl.egg-info/top_level.txt
```

### Comparing `seppl-0.2.0/CHANGES.rst` & `seppl-0.2.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+0.2.1 (2024-05-01)
+------------------
+
+- `ClassListerRegistry` now removes any excluded class listers before locating the classes
+
+
 0.2.0 (2024-05-01)
 ------------------
 
 - the `execute` method no longer counts `None` items returned by the reader
 - added the `seppl.ClassListerRegistry` class that offers a more convenient way of
   discovering classes via a function that returns a dictionary of superclasses and
   the associated modules to inspect; with this approach only a single entry_point
```

### Comparing `seppl-0.2.0/DESCRIPTION.rst` & `seppl-0.2.1/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/PKG-INFO` & `seppl-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: seppl
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python3 library for parsing pipeline components with their own options.
 Home-page: https://github.com/waikato-datamining/seppl
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: Simple Entry Point PipeLines (seppl). Python library for parsing pipeline components with their own options. 
         
@@ -18,14 +18,20 @@
         
         `https://github.com/waikato-datamining/seppl <https://github.com/waikato-datamining/seppl>`__
         
         
         Changelog
         =========
         
+        0.2.1 (2024-05-01)
+        ------------------
+        
+        - `ClassListerRegistry` now removes any excluded class listers before locating the classes
+        
+        
         0.2.0 (2024-05-01)
         ------------------
         
         - the `execute` method no longer counts `None` items returned by the reader
         - added the `seppl.ClassListerRegistry` class that offers a more convenient way of
           discovering classes via a function that returns a dictionary of superclasses and
           the associated modules to inspect; with this approach only a single entry_point
```

### Comparing `seppl-0.2.0/README.md` & `seppl-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/setup.py` & `seppl-0.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         'Programming Language :: Python :: 3',
     ],
     license='MIT License',
     package_dir={
         '': 'src'
     },
     packages=find_namespace_packages(where='src'),
-    version="0.2.0",
+    version="0.2.1",
     author='Peter Reutemann',
     author_email='fracpete@waikato.ac.nz',
     entry_points={
         "console_scripts": [
             "seppl-escape=seppl.tool.escape:sys_main",
             "seppl-unescape=seppl.tool.unescape:sys_main",
         ],
```

### Comparing `seppl-0.2.0/src/seppl/__init__.py` & `seppl-0.2.1/src/seppl/__init__.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl/_args.py` & `seppl-0.2.1/src/seppl/_args.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl/_class_registry.py` & `seppl-0.2.1/src/seppl/_class_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,18 @@
         # from entry points
         entry_point_classes = self._determine_from_entry_points(c)
         if entry_point_classes is not None:
             all_classes.update(entry_point_classes)
 
         # register from class listers as well?
         if (len(all_classes) == 0) or ((self._custom_class_listers is not None) and (len(self._custom_class_listers) > 0)) or self.has_env_class_listers():
-            all_classes.update(self._determine_from_class_listers(c, self.actual_fallback_class_listers()))
+            actual = self.actual_fallback_class_listers()
+            for excl in self.actual_excluded_class_listers():
+                actual.remove(excl)
+            all_classes.update(self._determine_from_class_listers(c, actual))
 
         self._classes[c] = sorted(list(all_classes))
 
     def plugins(self, c: Union[str, Type], fail_if_empty: bool = True) -> Dict[str, Plugin]:
         """
         Returns the classes for the specified superclass.
```

### Comparing `seppl-0.2.0/src/seppl/_entry_points.py` & `seppl-0.2.1/src/seppl/_entry_points.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl/_help.py` & `seppl-0.2.1/src/seppl/_help.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl/_metadata.py` & `seppl-0.2.1/src/seppl/_metadata.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl/_plugin.py` & `seppl-0.2.1/src/seppl/_plugin.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl/_registry.py` & `seppl-0.2.1/src/seppl/_registry.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl/_session.py` & `seppl-0.2.1/src/seppl/_session.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl/_types.py` & `seppl-0.2.1/src/seppl/_types.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl/io/_execution.py` & `seppl-0.2.1/src/seppl/io/_execution.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl/io/_filter.py` & `seppl-0.2.1/src/seppl/io/_filter.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl/io/_reader.py` & `seppl-0.2.1/src/seppl/io/_reader.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl/io/_split.py` & `seppl-0.2.1/src/seppl/io/_split.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl/io/_utils.py` & `seppl-0.2.1/src/seppl/io/_utils.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl/io/_writer.py` & `seppl-0.2.1/src/seppl/io/_writer.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl/tool/escape.py` & `seppl-0.2.1/src/seppl/tool/escape.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl/tool/unescape.py` & `seppl-0.2.1/src/seppl/tool/unescape.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.0/src/seppl.egg-info/PKG-INFO` & `seppl-0.2.1/src/seppl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: seppl
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python3 library for parsing pipeline components with their own options.
 Home-page: https://github.com/waikato-datamining/seppl
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: Simple Entry Point PipeLines (seppl). Python library for parsing pipeline components with their own options. 
         
@@ -18,14 +18,20 @@
         
         `https://github.com/waikato-datamining/seppl <https://github.com/waikato-datamining/seppl>`__
         
         
         Changelog
         =========
         
+        0.2.1 (2024-05-01)
+        ------------------
+        
+        - `ClassListerRegistry` now removes any excluded class listers before locating the classes
+        
+        
         0.2.0 (2024-05-01)
         ------------------
         
         - the `execute` method no longer counts `None` items returned by the reader
         - added the `seppl.ClassListerRegistry` class that offers a more convenient way of
           discovering classes via a function that returns a dictionary of superclasses and
           the associated modules to inspect; with this approach only a single entry_point
```

### Comparing `seppl-0.2.0/src/seppl.egg-info/SOURCES.txt` & `seppl-0.2.1/src/seppl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

