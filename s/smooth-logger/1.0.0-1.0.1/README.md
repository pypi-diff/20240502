# Comparing `tmp/smooth_logger-1.0.0.tar.gz` & `tmp/smooth_logger-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smooth_logger-1.0.0.tar", last modified: Wed May  1 11:42:06 2024, max compression
+gzip compressed data, was "smooth_logger-1.0.1.tar", last modified: Thu May  2 13:50:01 2024, max compression
```

## Comparing `smooth_logger-1.0.0.tar` & `smooth_logger-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-05-01 11:42:06.700392 smooth_logger-1.0.0/
--rw-r--r--   0 murdo      (502) murdo      (502)    34020 2022-08-16 10:25:55.000000 smooth_logger-1.0.0/LICENSE
--rw-r--r--   0 murdo      (502) murdo      (502)     6813 2024-05-01 11:42:06.700392 smooth_logger-1.0.0/PKG-INFO
--rw-r--r--   0 murdo      (502) murdo      (502)     5878 2024-05-01 11:28:58.000000 smooth_logger-1.0.0/README.md
--rw-r--r--   0 murdo      (502) murdo      (502)       38 2024-05-01 11:42:06.700392 smooth_logger-1.0.0/setup.cfg
--rw-r--r--   0 murdo      (502) murdo      (502)     1183 2024-05-01 11:29:32.000000 smooth_logger-1.0.0/setup.py
-drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-05-01 11:42:06.699392 smooth_logger-1.0.0/smooth_logger/
--rw-r--r--   0 murdo      (502) murdo      (502)      470 2024-05-01 10:21:37.000000 smooth_logger-1.0.0/smooth_logger/LogEntry.py
--rw-r--r--   0 murdo      (502) murdo      (502)    13010 2024-05-01 11:18:19.000000 smooth_logger-1.0.0/smooth_logger/Logger.py
--rw-r--r--   0 murdo      (502) murdo      (502)       89 2024-05-01 10:24:22.000000 smooth_logger-1.0.0/smooth_logger/__init__.py
--rw-r--r--   0 murdo      (502) murdo      (502)      376 2024-05-01 11:03:37.000000 smooth_logger-1.0.0/smooth_logger/enums.py
-drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-05-01 11:42:06.700392 smooth_logger-1.0.0/smooth_logger.egg-info/
--rw-r--r--   0 murdo      (502) murdo      (502)     6813 2024-05-01 11:42:06.000000 smooth_logger-1.0.0/smooth_logger.egg-info/PKG-INFO
--rw-r--r--   0 murdo      (502) murdo      (502)      309 2024-05-01 11:42:06.000000 smooth_logger-1.0.0/smooth_logger.egg-info/SOURCES.txt
--rw-r--r--   0 murdo      (502) murdo      (502)        1 2024-05-01 11:42:06.000000 smooth_logger-1.0.0/smooth_logger.egg-info/dependency_links.txt
--rw-r--r--   0 murdo      (502) murdo      (502)        6 2024-05-01 11:42:06.000000 smooth_logger-1.0.0/smooth_logger.egg-info/requires.txt
--rw-r--r--   0 murdo      (502) murdo      (502)       14 2024-05-01 11:42:06.000000 smooth_logger-1.0.0/smooth_logger.egg-info/top_level.txt
+drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-05-02 13:50:01.685986 smooth_logger-1.0.1/
+-rw-r--r--   0 murdo      (502) murdo      (502)    34020 2022-08-16 10:25:55.000000 smooth_logger-1.0.1/LICENSE
+-rw-r--r--   0 murdo      (502) murdo      (502)     6813 2024-05-02 13:50:01.685986 smooth_logger-1.0.1/PKG-INFO
+-rw-r--r--   0 murdo      (502) murdo      (502)     5878 2024-05-01 11:49:38.000000 smooth_logger-1.0.1/README.md
+-rw-r--r--   0 murdo      (502) murdo      (502)       38 2024-05-02 13:50:01.685986 smooth_logger-1.0.1/setup.cfg
+-rw-r--r--   0 murdo      (502) murdo      (502)     1183 2024-05-02 13:48:46.000000 smooth_logger-1.0.1/setup.py
+drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-05-02 13:50:01.684986 smooth_logger-1.0.1/smooth_logger/
+-rw-r--r--   0 murdo      (502) murdo      (502)      470 2024-05-01 10:21:37.000000 smooth_logger-1.0.1/smooth_logger/LogEntry.py
+-rw-r--r--   0 murdo      (502) murdo      (502)    13002 2024-05-02 13:46:28.000000 smooth_logger-1.0.1/smooth_logger/Logger.py
+-rw-r--r--   0 murdo      (502) murdo      (502)       89 2024-05-01 10:24:22.000000 smooth_logger-1.0.1/smooth_logger/__init__.py
+-rw-r--r--   0 murdo      (502) murdo      (502)      376 2024-05-01 11:03:37.000000 smooth_logger-1.0.1/smooth_logger/enums.py
+drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-05-02 13:50:01.685986 smooth_logger-1.0.1/smooth_logger.egg-info/
+-rw-r--r--   0 murdo      (502) murdo      (502)     6813 2024-05-02 13:50:01.000000 smooth_logger-1.0.1/smooth_logger.egg-info/PKG-INFO
+-rw-r--r--   0 murdo      (502) murdo      (502)      309 2024-05-02 13:50:01.000000 smooth_logger-1.0.1/smooth_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 murdo      (502) murdo      (502)        1 2024-05-02 13:50:01.000000 smooth_logger-1.0.1/smooth_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 murdo      (502) murdo      (502)        6 2024-05-02 13:50:01.000000 smooth_logger-1.0.1/smooth_logger.egg-info/requires.txt
+-rw-r--r--   0 murdo      (502) murdo      (502)       14 2024-05-02 13:50:01.000000 smooth_logger-1.0.1/smooth_logger.egg-info/top_level.txt
```

### Comparing `smooth_logger-1.0.0/LICENSE` & `smooth_logger-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smooth_logger-1.0.0/PKG-INFO` & `smooth_logger-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smooth_logger
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple logger made primarily for my own personal use. Made from a combination of necessity and so much sloth that it overflowed into productivity.
 Home-page: https://github.com/MurdoMaclachlan/smooth_logger
 Author: Murdo Maclachlan
 Author-email: murdomaclachlan@duck.com
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `smooth_logger-1.0.0/README.md` & `smooth_logger-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `smooth_logger-1.0.0/setup.py` & `smooth_logger-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     return open('README.md', 'r').read()
 
 
 setup(
     name="smooth_logger",
-    version="1.0.0",
+    version="1.0.1",
     author="Murdo Maclachlan",
     author_email="murdomaclachlan@duck.com",
     description=(
         "A simple logger made primarily for my own personal use. Made from a combination of"
         + " necessity and so much sloth that it overflowed into productivity."
     ),
     long_description=readme(),
```

### Comparing `smooth_logger-1.0.0/smooth_logger/Logger.py` & `smooth_logger-1.0.1/smooth_logger/Logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
             output: bool = (
                 False
                 if scope is None else
                 self._scopes[scope] in [Categories.MAXIMUM, Categories.SAVE]
             )
             
             entry: LogEntry = self.__create_log_entry(message, output, scope)
-            self.__display_log_entry(entry, scope, notify, is_bar, print_to_console)
+            self.__display_log_entry(entry, scope, notify, print_to_console)
 
             self.__write_logs = self.__write_logs or output
             self.is_empty = False
 
             return True
         else:
             self.new("Unknown scope passed to Logger.new()", "WARNING")
```

### Comparing `smooth_logger-1.0.0/smooth_logger.egg-info/PKG-INFO` & `smooth_logger-1.0.1/smooth_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smooth_logger
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple logger made primarily for my own personal use. Made from a combination of necessity and so much sloth that it overflowed into productivity.
 Home-page: https://github.com/MurdoMaclachlan/smooth_logger
 Author: Murdo Maclachlan
 Author-email: murdomaclachlan@duck.com
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.7
```

