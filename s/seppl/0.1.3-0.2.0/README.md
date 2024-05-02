# Comparing `tmp/seppl-0.1.3.tar.gz` & `tmp/seppl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seppl-0.1.3.tar", last modified: Wed Feb 28 20:11:23 2024, max compression
+gzip compressed data, was "seppl-0.2.0.tar", last modified: Wed May  1 03:41:31 2024, max compression
```

## Comparing `seppl-0.1.3.tar` & `seppl-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-28 20:11:23.164102 seppl-0.1.3/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3615 2024-02-28 20:08:15.000000 seppl-0.1.3/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      568 2023-11-09 01:56:09.000000 seppl-0.1.3/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 seppl-0.1.3/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5728 2024-02-28 20:11:23.164102 seppl-0.1.3/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    11402 2024-02-28 20:10:38.000000 seppl-0.1.3/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2024-02-28 20:11:23.164102 seppl-0.1.3/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1130 2024-02-28 20:08:15.000000 seppl-0.1.3/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-28 20:11:23.160102 seppl-0.1.3/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-28 20:11:23.164102 seppl-0.1.3/src/seppl/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      689 2024-02-28 19:34:57.000000 seppl-0.1.3/src/seppl/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5702 2024-02-21 21:20:08.000000 seppl-0.1.3/src/seppl/_args.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1719 2023-10-04 19:59:54.000000 seppl-0.1.3/src/seppl/_entry_points.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2876 2023-10-04 20:28:17.000000 seppl-0.1.3/src/seppl/_help.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1942 2024-02-04 21:21:35.000000 seppl-0.1.3/src/seppl/_metadata.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8347 2024-02-28 19:32:25.000000 seppl-0.1.3/src/seppl/_plugin.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    15741 2023-11-26 19:45:43.000000 seppl-0.1.3/src/seppl/_registry.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1679 2024-02-04 21:33:05.000000 seppl-0.1.3/src/seppl/_session.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2623 2024-02-28 19:32:25.000000 seppl-0.1.3/src/seppl/_types.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-28 20:11:23.164102 seppl-0.1.3/src/seppl/io/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      282 2024-02-05 00:23:10.000000 seppl-0.1.3/src/seppl/io/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5241 2024-02-05 00:16:01.000000 seppl-0.1.3/src/seppl/io/_execution.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6560 2024-02-04 23:34:50.000000 seppl-0.1.3/src/seppl/io/_filter.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1555 2024-02-04 23:40:54.000000 seppl-0.1.3/src/seppl/io/_reader.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3147 2024-02-07 03:48:04.000000 seppl-0.1.3/src/seppl/io/_split.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2444 2024-02-05 00:23:10.000000 seppl-0.1.3/src/seppl/io/_utils.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3319 2024-02-04 23:40:54.000000 seppl-0.1.3/src/seppl/io/_writer.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-28 20:11:23.164102 seppl-0.1.3/src/seppl/tool/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2024-02-21 20:25:44.000000 seppl-0.1.3/src/seppl/tool/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      772 2024-02-21 20:32:02.000000 seppl-0.1.3/src/seppl/tool/escape.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      780 2024-02-21 20:32:02.000000 seppl-0.1.3/src/seppl/tool/unescape.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-28 20:11:23.164102 seppl-0.1.3/src/seppl.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5728 2024-02-28 20:11:23.000000 seppl-0.1.3/src/seppl.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      671 2024-02-28 20:11:23.000000 seppl-0.1.3/src/seppl.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2024-02-28 20:11:23.000000 seppl-0.1.3/src/seppl.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      107 2024-02-28 20:11:23.000000 seppl-0.1.3/src/seppl.egg-info/entry_points.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        6 2024-02-28 20:11:23.000000 seppl-0.1.3/src/seppl.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-01 03:41:31.413744 seppl-0.2.0/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4060 2024-05-01 03:40:48.000000 seppl-0.2.0/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      568 2023-11-09 01:56:09.000000 seppl-0.2.0/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 seppl-0.2.0/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6253 2024-05-01 03:41:31.413744 seppl-0.2.0/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3741 2024-05-01 03:08:55.000000 seppl-0.2.0/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2024-05-01 03:41:31.413744 seppl-0.2.0/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1130 2024-05-01 03:40:48.000000 seppl-0.2.0/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-01 03:41:31.409744 seppl-0.2.0/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-01 03:41:31.413744 seppl-0.2.0/src/seppl/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      765 2024-04-30 23:53:36.000000 seppl-0.2.0/src/seppl/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5702 2024-02-21 21:20:08.000000 seppl-0.2.0/src/seppl/_args.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    16420 2024-05-01 01:31:12.000000 seppl-0.2.0/src/seppl/_class_registry.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1719 2023-10-04 19:59:54.000000 seppl-0.2.0/src/seppl/_entry_points.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2876 2023-10-04 20:28:17.000000 seppl-0.2.0/src/seppl/_help.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1942 2024-02-04 21:21:35.000000 seppl-0.2.0/src/seppl/_metadata.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8347 2024-02-28 19:32:25.000000 seppl-0.2.0/src/seppl/_plugin.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    15743 2024-04-30 23:41:51.000000 seppl-0.2.0/src/seppl/_registry.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1679 2024-02-04 21:33:05.000000 seppl-0.2.0/src/seppl/_session.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2623 2024-02-28 19:32:25.000000 seppl-0.2.0/src/seppl/_types.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-01 03:41:31.413744 seppl-0.2.0/src/seppl/io/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      282 2024-02-05 00:23:10.000000 seppl-0.2.0/src/seppl/io/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5553 2024-03-21 01:02:31.000000 seppl-0.2.0/src/seppl/io/_execution.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6560 2024-02-04 23:34:50.000000 seppl-0.2.0/src/seppl/io/_filter.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1555 2024-02-04 23:40:54.000000 seppl-0.2.0/src/seppl/io/_reader.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3147 2024-02-07 03:48:04.000000 seppl-0.2.0/src/seppl/io/_split.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2444 2024-02-05 00:23:10.000000 seppl-0.2.0/src/seppl/io/_utils.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3319 2024-02-04 23:40:54.000000 seppl-0.2.0/src/seppl/io/_writer.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-01 03:41:31.413744 seppl-0.2.0/src/seppl/tool/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2024-02-21 20:25:44.000000 seppl-0.2.0/src/seppl/tool/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      772 2024-02-21 20:32:02.000000 seppl-0.2.0/src/seppl/tool/escape.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      780 2024-02-21 20:32:02.000000 seppl-0.2.0/src/seppl/tool/unescape.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-01 03:41:31.413744 seppl-0.2.0/src/seppl.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6253 2024-05-01 03:41:31.000000 seppl-0.2.0/src/seppl.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      700 2024-05-01 03:41:31.000000 seppl-0.2.0/src/seppl.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2024-05-01 03:41:31.000000 seppl-0.2.0/src/seppl.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      107 2024-05-01 03:41:31.000000 seppl-0.2.0/src/seppl.egg-info/entry_points.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        6 2024-05-01 03:41:31.000000 seppl-0.2.0/src/seppl.egg-info/top_level.txt
```

### Comparing `seppl-0.1.3/CHANGES.rst` & `seppl-0.2.0/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+0.2.0 (2024-05-01)
+------------------
+
+- the `execute` method no longer counts `None` items returned by the reader
+- added the `seppl.ClassListerRegistry` class that offers a more convenient way of
+  discovering classes via a function that returns a dictionary of superclasses and
+  the associated modules to inspect; with this approach only a single entry_point
+  has to be defined in `setup.py`, pointing to the class lister module/function
+
+
 0.1.3 (2024-02-29)
 ------------------
 
 - added the dummy type `AnyData` which is used by default in the `check_compatibility`
   method for a *match all* (ie can be used for general purpose plugins)
```

### Comparing `seppl-0.1.3/DESCRIPTION.rst` & `seppl-0.2.0/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `seppl-0.1.3/PKG-INFO` & `seppl-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: seppl
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python3 library for parsing pipeline components with their own options.
 Home-page: https://github.com/waikato-datamining/seppl
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: Simple Entry Point PipeLines (seppl). Python library for parsing pipeline components with their own options. 
         
@@ -18,14 +18,24 @@
         
         `https://github.com/waikato-datamining/seppl <https://github.com/waikato-datamining/seppl>`__
         
         
         Changelog
         =========
         
+        0.2.0 (2024-05-01)
+        ------------------
+        
+        - the `execute` method no longer counts `None` items returned by the reader
+        - added the `seppl.ClassListerRegistry` class that offers a more convenient way of
+          discovering classes via a function that returns a dictionary of superclasses and
+          the associated modules to inspect; with this approach only a single entry_point
+          has to be defined in `setup.py`, pointing to the class lister module/function
+        
+        
         0.1.3 (2024-02-29)
         ------------------
         
         - added the dummy type `AnyData` which is used by default in the `check_compatibility`
           method for a *match all* (ie can be used for general purpose plugins)
```

### Comparing `seppl-0.1.3/setup.py` & `seppl-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         'Programming Language :: Python :: 3',
     ],
     license='MIT License',
     package_dir={
         '': 'src'
     },
     packages=find_namespace_packages(where='src'),
-    version="0.1.3",
+    version="0.2.0",
     author='Peter Reutemann',
     author_email='fracpete@waikato.ac.nz',
     entry_points={
         "console_scripts": [
             "seppl-escape=seppl.tool.escape:sys_main",
             "seppl-unescape=seppl.tool.unescape:sys_main",
         ],
```

### Comparing `seppl-0.1.3/src/seppl/_args.py` & `seppl-0.2.0/src/seppl/_args.py`

 * *Files identical despite different names*

### Comparing `seppl-0.1.3/src/seppl/_entry_points.py` & `seppl-0.2.0/src/seppl/_entry_points.py`

 * *Files identical despite different names*

### Comparing `seppl-0.1.3/src/seppl/_help.py` & `seppl-0.2.0/src/seppl/_help.py`

 * *Files identical despite different names*

### Comparing `seppl-0.1.3/src/seppl/_metadata.py` & `seppl-0.2.0/src/seppl/_metadata.py`

 * *Files identical despite different names*

### Comparing `seppl-0.1.3/src/seppl/_plugin.py` & `seppl-0.2.0/src/seppl/_plugin.py`

 * *Files identical despite different names*

### Comparing `seppl-0.1.3/src/seppl/_registry.py` & `seppl-0.2.0/src/seppl/_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,7 +443,9 @@
         :param c: the class that the plugins must be, any class derived from Plugin if None
         :return: the dictionary of plugins (name / plugin association)
         :rtype: dict
         """
         if group not in self._plugins:
             self._register(group, c)
         return self._plugins[group]
+
+
```

### Comparing `seppl-0.1.3/src/seppl/_session.py` & `seppl-0.2.0/src/seppl/_session.py`

 * *Files identical despite different names*

### Comparing `seppl-0.1.3/src/seppl/_types.py` & `seppl-0.2.0/src/seppl/_types.py`

 * *Files identical despite different names*

### Comparing `seppl-0.1.3/src/seppl/io/_execution.py` & `seppl-0.2.0/src/seppl/io/_execution.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,23 +51,27 @@
     # process data
     try:
         while not reader.has_finished():
             if isinstance(writer, BatchWriter):
                 data = []
                 if session.options.force_batch:
                     for item in reader.read():
+                        if item is None:
+                            continue
                         session.count += 1
                         data.append(item)
                         if session.count % session.options.update_interval == 0:
                             session.logger.info("%d records read..." % session.count)
                     if filter_ is not None:
                         data = filter_.process(data)
                         session.logger.info("%d records filtered..." % session.count)
                 else:
                     for item in reader.read():
+                        if item is None:
+                            continue
                         session.count += 1
                         if (filter_ is not None) and (item is not None):
                             item = filter_.process(item)
                         if item is not None:
                             if not isinstance(item, list):
                                 item = [item]
                             data.extend(item)
@@ -75,14 +79,16 @@
                             session.logger.info("%d records processed..." % session.count)
                 writer.write_batch(data)
                 session.logger.info("%d records processed in total." % session.count)
             elif isinstance(writer, StreamWriter) or (writer is None):
                 if session.options.force_batch:
                     data = []
                     for item in reader.read():
+                        if item is None:
+                            continue
                         session.count += 1
                         data.append(item)
                         if session.count % session.options.update_interval == 0:
                             session.logger.info("%d records read..." % session.count)
                     if filter_ is not None:
                         count = len(data)
                         data = filter_.process(data)
@@ -94,14 +100,16 @@
                         for item in data:
                             count += 1
                             writer.write_stream(item)
                             if count % session.options.update_interval == 0:
                                 session.logger.info("%d records written..." % count)
                 else:
                     for item in reader.read():
+                        if item is None:
+                            continue
                         session.count += 1
                         if (filter_ is not None) and (item is not None):
                             item = filter_.process(item)
                         if item is not None:
                             if writer is not None:
                                 writer.write_stream(item)
                         if session.count % session.options.update_interval == 0:
```

### Comparing `seppl-0.1.3/src/seppl/io/_filter.py` & `seppl-0.2.0/src/seppl/io/_filter.py`

 * *Files identical despite different names*

### Comparing `seppl-0.1.3/src/seppl/io/_reader.py` & `seppl-0.2.0/src/seppl/io/_reader.py`

 * *Files identical despite different names*

### Comparing `seppl-0.1.3/src/seppl/io/_split.py` & `seppl-0.2.0/src/seppl/io/_split.py`

 * *Files identical despite different names*

### Comparing `seppl-0.1.3/src/seppl/io/_utils.py` & `seppl-0.2.0/src/seppl/io/_utils.py`

 * *Files identical despite different names*

### Comparing `seppl-0.1.3/src/seppl/io/_writer.py` & `seppl-0.2.0/src/seppl/io/_writer.py`

 * *Files identical despite different names*

### Comparing `seppl-0.1.3/src/seppl/tool/escape.py` & `seppl-0.2.0/src/seppl/tool/escape.py`

 * *Files identical despite different names*

### Comparing `seppl-0.1.3/src/seppl/tool/unescape.py` & `seppl-0.2.0/src/seppl/tool/unescape.py`

 * *Files identical despite different names*

### Comparing `seppl-0.1.3/src/seppl.egg-info/PKG-INFO` & `seppl-0.2.0/src/seppl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: seppl
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python3 library for parsing pipeline components with their own options.
 Home-page: https://github.com/waikato-datamining/seppl
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: Simple Entry Point PipeLines (seppl). Python library for parsing pipeline components with their own options. 
         
@@ -18,14 +18,24 @@
         
         `https://github.com/waikato-datamining/seppl <https://github.com/waikato-datamining/seppl>`__
         
         
         Changelog
         =========
         
+        0.2.0 (2024-05-01)
+        ------------------
+        
+        - the `execute` method no longer counts `None` items returned by the reader
+        - added the `seppl.ClassListerRegistry` class that offers a more convenient way of
+          discovering classes via a function that returns a dictionary of superclasses and
+          the associated modules to inspect; with this approach only a single entry_point
+          has to be defined in `setup.py`, pointing to the class lister module/function
+        
+        
         0.1.3 (2024-02-29)
         ------------------
         
         - added the dummy type `AnyData` which is used by default in the `check_compatibility`
           method for a *match all* (ie can be used for general purpose plugins)
```

### Comparing `seppl-0.1.3/src/seppl.egg-info/SOURCES.txt` & `seppl-0.2.0/src/seppl.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 CHANGES.rst
 DESCRIPTION.rst
 MANIFEST.in
 README.md
 setup.py
 src/seppl/__init__.py
 src/seppl/_args.py
+src/seppl/_class_registry.py
 src/seppl/_entry_points.py
 src/seppl/_help.py
 src/seppl/_metadata.py
 src/seppl/_plugin.py
 src/seppl/_registry.py
 src/seppl/_session.py
 src/seppl/_types.py
```

