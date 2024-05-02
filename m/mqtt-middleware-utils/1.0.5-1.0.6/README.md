# Comparing `tmp/mqtt_middleware_utils-1.0.5.tar.gz` & `tmp/mqtt_middleware_utils-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt_middleware_utils-1.0.5.tar", last modified: Fri Nov 10 10:47:24 2023, max compression
+gzip compressed data, was "mqtt_middleware_utils-1.0.6.tar", last modified: Thu May  2 10:02:38 2024, max compression
```

## Comparing `mqtt_middleware_utils-1.0.5.tar` & `mqtt_middleware_utils-1.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-11-10 10:47:24.869178 mqtt_middleware_utils-1.0.5/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35148 2023-10-23 09:27:12.000000 mqtt_middleware_utils-1.0.5/LICENSE.txt
--rw-r--r--   0 andrea    (1000) andrea    (1000)      667 2023-11-10 10:47:24.869178 mqtt_middleware_utils-1.0.5/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      115 2023-10-09 07:21:51.000000 mqtt_middleware_utils-1.0.5/README.md
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-11-10 10:47:24.869178 mqtt_middleware_utils-1.0.5/mqtt_middleware_utils.egg-info/
--rw-r--r--   0 andrea    (1000) andrea    (1000)      667 2023-11-10 10:47:24.000000 mqtt_middleware_utils-1.0.5/mqtt_middleware_utils.egg-info/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      571 2023-11-10 10:47:24.000000 mqtt_middleware_utils-1.0.5/mqtt_middleware_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-11-10 10:47:24.000000 mqtt_middleware_utils-1.0.5/mqtt_middleware_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       41 2023-11-10 10:47:24.000000 mqtt_middleware_utils-1.0.5/mqtt_middleware_utils.egg-info/requires.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       21 2023-11-10 10:47:24.000000 mqtt_middleware_utils-1.0.5/mqtt_middleware_utils.egg-info/top_level.txt
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-11-10 10:47:24.869178 mqtt_middleware_utils-1.0.5/mqtt_middlware_utils/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-10-09 07:21:51.000000 mqtt_middleware_utils-1.0.5/mqtt_middlware_utils/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    11601 2023-11-08 10:12:59.000000 mqtt_middleware_utils-1.0.5/mqtt_middlware_utils/db_utils.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-11-10 10:47:24.869178 mqtt_middleware_utils-1.0.5/mqtt_middlware_utils/exceptions/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-10-09 07:21:51.000000 mqtt_middleware_utils-1.0.5/mqtt_middlware_utils/exceptions/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2107 2023-10-16 07:39:49.000000 mqtt_middleware_utils-1.0.5/mqtt_middlware_utils/exceptions/mqtt_middleware_exceptions.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3666 2023-10-16 07:39:49.000000 mqtt_middleware_utils-1.0.5/mqtt_middlware_utils/logging_utils.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7616 2023-11-10 10:46:44.000000 mqtt_middleware_utils-1.0.5/mqtt_middlware_utils/utils.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      608 2023-11-10 10:46:44.000000 mqtt_middleware_utils-1.0.5/pyproject.toml
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2023-11-10 10:47:24.869178 mqtt_middleware_utils-1.0.5/setup.cfg
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-11-10 10:47:24.869178 mqtt_middleware_utils-1.0.5/tests/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    23577 2023-11-08 10:12:59.000000 mqtt_middleware_utils-1.0.5/tests/test_db_utils.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6477 2023-10-16 07:39:49.000000 mqtt_middleware_utils-1.0.5/tests/test_logging_utils.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    16452 2023-11-10 10:46:44.000000 mqtt_middleware_utils-1.0.5/tests/test_utils.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-02 10:02:38.783273 mqtt_middleware_utils-1.0.6/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35148 2023-10-23 09:27:12.000000 mqtt_middleware_utils-1.0.6/LICENSE.txt
+-rw-r--r--   0 andrea    (1000) andrea    (1000)      667 2024-05-02 10:02:38.783273 mqtt_middleware_utils-1.0.6/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      115 2023-10-09 07:21:51.000000 mqtt_middleware_utils-1.0.6/README.md
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-02 10:02:38.783273 mqtt_middleware_utils-1.0.6/mqtt_middleware_utils.egg-info/
+-rw-r--r--   0 andrea    (1000) andrea    (1000)      667 2024-05-02 10:02:38.000000 mqtt_middleware_utils-1.0.6/mqtt_middleware_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      571 2024-05-02 10:02:38.000000 mqtt_middleware_utils-1.0.6/mqtt_middleware_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2024-05-02 10:02:38.000000 mqtt_middleware_utils-1.0.6/mqtt_middleware_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       41 2024-05-02 10:02:38.000000 mqtt_middleware_utils-1.0.6/mqtt_middleware_utils.egg-info/requires.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       21 2024-05-02 10:02:38.000000 mqtt_middleware_utils-1.0.6/mqtt_middleware_utils.egg-info/top_level.txt
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-02 10:02:38.783273 mqtt_middleware_utils-1.0.6/mqtt_middlware_utils/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-10-09 07:21:51.000000 mqtt_middleware_utils-1.0.6/mqtt_middlware_utils/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    11909 2024-05-02 09:59:44.000000 mqtt_middleware_utils-1.0.6/mqtt_middlware_utils/db_utils.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-02 10:02:38.783273 mqtt_middleware_utils-1.0.6/mqtt_middlware_utils/exceptions/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-10-09 07:21:51.000000 mqtt_middleware_utils-1.0.6/mqtt_middlware_utils/exceptions/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2107 2023-10-16 07:39:49.000000 mqtt_middleware_utils-1.0.6/mqtt_middlware_utils/exceptions/mqtt_middleware_exceptions.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3666 2023-10-16 07:39:49.000000 mqtt_middleware_utils-1.0.6/mqtt_middlware_utils/logging_utils.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7616 2023-11-10 10:46:44.000000 mqtt_middleware_utils-1.0.6/mqtt_middlware_utils/utils.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      608 2024-05-02 10:01:45.000000 mqtt_middleware_utils-1.0.6/pyproject.toml
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2024-05-02 10:02:38.783273 mqtt_middleware_utils-1.0.6/setup.cfg
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-02 10:02:38.783273 mqtt_middleware_utils-1.0.6/tests/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    23577 2023-11-08 10:12:59.000000 mqtt_middleware_utils-1.0.6/tests/test_db_utils.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6477 2023-10-16 07:39:49.000000 mqtt_middleware_utils-1.0.6/tests/test_logging_utils.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    16452 2023-11-10 10:46:44.000000 mqtt_middleware_utils-1.0.6/tests/test_utils.py
```

### Comparing `mqtt_middleware_utils-1.0.5/LICENSE.txt` & `mqtt_middleware_utils-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mqtt_middleware_utils-1.0.5/PKG-INFO` & `mqtt_middleware_utils-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt_middleware_utils
-Version: 1.0.5
+Version: 1.0.6
 Summary: MQTT Middleware package containing all functions that must be shared between FaaS projects
 Author-email: Andrea Ranfone <andrea.ranfone@top-network.it>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
```

### Comparing `mqtt_middleware_utils-1.0.5/mqtt_middleware_utils.egg-info/PKG-INFO` & `mqtt_middleware_utils-1.0.6/mqtt_middleware_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mqtt-middleware-utils
-Version: 1.0.5
+Name: mqtt_middleware_utils
+Version: 1.0.6
 Summary: MQTT Middleware package containing all functions that must be shared between FaaS projects
 Author-email: Andrea Ranfone <andrea.ranfone@top-network.it>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
```

### Comparing `mqtt_middleware_utils-1.0.5/mqtt_middleware_utils.egg-info/SOURCES.txt` & `mqtt_middleware_utils-1.0.6/mqtt_middleware_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mqtt_middleware_utils-1.0.5/mqtt_middlware_utils/db_utils.py` & `mqtt_middleware_utils-1.0.6/mqtt_middlware_utils/db_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,28 +200,33 @@
         raise DatabaseCreateIndexError(
             "The following error occurred trying to create the index [(index_name: " +
             str(index_name) + ") (schema: "+str(schema)+") (definition: "+str(definition) +
             ")]: \n"+str(e))
 
 
 @db_exceptions_decorator
-def search_from_index(connection, index_name, query_string="*"):
+def search_from_index(connection, index_name, query_string="*", offset=None, num=None):
     '''
     Performs a search on the index using the provided query string
 
-    @param connection: the database connection
-    @param index_name: the name of the index to search on
-    @param query_string: the query string to use, if default searches all index
+    @param connection: the database connection (mandatory)
+    @param index_name: the name of the index to search on (mandatory)
+    @param query_string: the query string to use, if default searches all index (mandatory)
+    @param offset: the offset from where to start returning results (optional)
+    @param num: the number of results to return (optional)
 
     @return: the results of the search
 
     @raise DatabaseIndexSearchError if an error occurrs during the search operation on the index.
     '''
     try:
-        return connection.ft(index_name).search(Query(query_string))
+        query = Query(query_string)
+        if offset is not None and num is not None:
+            query.paging(offset, num)
+        return connection.ft(index_name).search(query)
     except Exception as e:
         raise DatabaseIndexSearchError(
             "The following error occurred trying to search the index [(index_name: " +
             str(index_name) + ") (query_string: "+str(query_string)+")]: \n"+str(e))
 
 
 @db_exceptions_decorator
```

### Comparing `mqtt_middleware_utils-1.0.5/mqtt_middlware_utils/exceptions/mqtt_middleware_exceptions.py` & `mqtt_middleware_utils-1.0.6/mqtt_middlware_utils/exceptions/mqtt_middleware_exceptions.py`

 * *Files identical despite different names*

### Comparing `mqtt_middleware_utils-1.0.5/mqtt_middlware_utils/logging_utils.py` & `mqtt_middleware_utils-1.0.6/mqtt_middlware_utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `mqtt_middleware_utils-1.0.5/mqtt_middlware_utils/utils.py` & `mqtt_middleware_utils-1.0.6/mqtt_middlware_utils/utils.py`

 * *Files identical despite different names*

### Comparing `mqtt_middleware_utils-1.0.5/pyproject.toml` & `mqtt_middleware_utils-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.2.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mqtt_middleware_utils"
-version = "1.0.5"
+version = "1.0.6"
 authors = [{ name = "Andrea Ranfone", email = "andrea.ranfone@top-network.it" }]
 description = "MQTT Middleware package containing all functions that must be shared between FaaS projects"
 readme = "README.md"
 requires-python = ">=3.8.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `mqtt_middleware_utils-1.0.5/tests/test_db_utils.py` & `mqtt_middleware_utils-1.0.6/tests/test_db_utils.py`

 * *Files identical despite different names*

### Comparing `mqtt_middleware_utils-1.0.5/tests/test_logging_utils.py` & `mqtt_middleware_utils-1.0.6/tests/test_logging_utils.py`

 * *Files identical despite different names*

### Comparing `mqtt_middleware_utils-1.0.5/tests/test_utils.py` & `mqtt_middleware_utils-1.0.6/tests/test_utils.py`

 * *Files identical despite different names*

