# Comparing `tmp/ixoncdkingress-0.0.8.tar.gz` & `tmp/ixoncdkingress-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixoncdkingress-0.0.8.tar", last modified: Mon Jul 10 09:55:59 2023, max compression
+gzip compressed data, was "ixoncdkingress-0.0.9.tar", last modified: Mon Jul 10 11:32:57 2023, max compression
```

## Comparing `ixoncdkingress-0.0.8.tar` & `ixoncdkingress-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:55:59.473914 ixoncdkingress-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      278 2023-07-10 09:55:59.473914 ixoncdkingress-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      871 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:55:59.469914 ixoncdkingress-0.0.8/ixoncdkingress/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:55:24.000000 ixoncdkingress-0.0.8/ixoncdkingress/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:55:59.473914 ixoncdkingress-0.0.8/ixoncdkingress/cbc/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:55:24.000000 ixoncdkingress-0.0.8/ixoncdkingress/cbc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8106 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/cbc/api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/cbc/caller.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/cbc/context.py
--rw-rw-rw-   0 root         (0) root         (0)     3922 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/cbc/document_db_client.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:55:24.000000 ixoncdkingress-0.0.8/ixoncdkingress/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     1111 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/types.py
--rw-rw-rw-   0 root         (0) root         (0)      476 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:55:59.473914 ixoncdkingress-0.0.8/ixoncdkingress/webserver/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:55:24.000000 ixoncdkingress-0.0.8/ixoncdkingress/webserver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4208 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/webserver/config.py
--rw-rw-rw-   0 root         (0) root         (0)     7687 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/webserver/form.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/webserver/request.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/webserver/response.py
--rw-rw-rw-   0 root         (0) root         (0)     4445 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/webserver/servlet.py
--rw-rw-rw-   0 root         (0) root         (0)     6425 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/webserver/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3462 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/webserver/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:55:59.473914 ixoncdkingress-0.0.8/ixoncdkingress.egg-info/
--rw-r--r--   0 root         (0) root         (0)      278 2023-07-10 09:55:59.000000 ixoncdkingress-0.0.8/ixoncdkingress.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      841 2023-07-10 09:55:59.000000 ixoncdkingress-0.0.8/ixoncdkingress.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 09:55:59.000000 ixoncdkingress-0.0.8/ixoncdkingress.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      264 2023-07-10 09:55:59.000000 ixoncdkingress-0.0.8/ixoncdkingress.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-10 09:55:59.000000 ixoncdkingress-0.0.8/ixoncdkingress.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 09:55:59.473914 ixoncdkingress-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      951 2023-07-10 09:55:59.000000 ixoncdkingress-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:55:59.473914 ixoncdkingress-0.0.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1055 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/tests/test___main__.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/tests/test_types.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:32:57.040148 ixoncdkingress-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      278 2023-07-10 11:32:57.040148 ixoncdkingress-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      871 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:32:57.016148 ixoncdkingress-0.0.9/ixoncdkingress/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 11:31:53.000000 ixoncdkingress-0.0.9/ixoncdkingress/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/ixoncdkingress/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:32:57.020148 ixoncdkingress-0.0.9/ixoncdkingress/cbc/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 11:31:53.000000 ixoncdkingress-0.0.9/ixoncdkingress/cbc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8106 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/ixoncdkingress/cbc/api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/ixoncdkingress/cbc/caller.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/ixoncdkingress/cbc/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     3928 2023-07-10 10:23:09.000000 ixoncdkingress-0.0.9/ixoncdkingress/cbc/document_db_client.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 11:31:53.000000 ixoncdkingress-0.0.9/ixoncdkingress/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     1111 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/ixoncdkingress/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      476 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/ixoncdkingress/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:32:57.040148 ixoncdkingress-0.0.9/ixoncdkingress/webserver/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 11:31:53.000000 ixoncdkingress-0.0.9/ixoncdkingress/webserver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4208 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/ixoncdkingress/webserver/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     7687 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/ixoncdkingress/webserver/form.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/ixoncdkingress/webserver/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/ixoncdkingress/webserver/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     4445 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/ixoncdkingress/webserver/servlet.py
+-rw-rw-rw-   0 root         (0) root         (0)     6425 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/ixoncdkingress/webserver/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3462 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/ixoncdkingress/webserver/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:32:57.016148 ixoncdkingress-0.0.9/ixoncdkingress.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      278 2023-07-10 11:32:56.000000 ixoncdkingress-0.0.9/ixoncdkingress.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      841 2023-07-10 11:32:57.000000 ixoncdkingress-0.0.9/ixoncdkingress.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 11:32:56.000000 ixoncdkingress-0.0.9/ixoncdkingress.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      264 2023-07-10 11:32:56.000000 ixoncdkingress-0.0.9/ixoncdkingress.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-10 11:32:56.000000 ixoncdkingress-0.0.9/ixoncdkingress.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 11:32:57.040148 ixoncdkingress-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-07-10 11:32:56.000000 ixoncdkingress-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:32:57.040148 ixoncdkingress-0.0.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1055 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/tests/test___main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/tests/test_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-07-10 09:54:47.000000 ixoncdkingress-0.0.9/tests/test_utils.py
```

### Comparing `ixoncdkingress-0.0.8/README.md` & `ixoncdkingress-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.8/ixoncdkingress/__main__.py` & `ixoncdkingress-0.0.9/ixoncdkingress/__main__.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.8/ixoncdkingress/cbc/api_client.py` & `ixoncdkingress-0.0.9/ixoncdkingress/cbc/api_client.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.8/ixoncdkingress/cbc/caller.py` & `ixoncdkingress-0.0.9/ixoncdkingress/cbc/caller.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.8/ixoncdkingress/cbc/context.py` & `ixoncdkingress-0.0.9/ixoncdkingress/cbc/context.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.8/ixoncdkingress/cbc/document_db_client.py` & `ixoncdkingress-0.0.9/ixoncdkingress/cbc/document_db_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,21 +113,21 @@
 
     def find_one(
         self, *args: Any, filter_map: Optional[Any], **kwargs: Any
     ) -> Optional[DocumentType]:
         """
         Get a single document from the database.
         """
-        return self._get_collection().find_one(filter_map, args, kwargs)
+        return self._get_collection().find_one(filter_map, *args, **kwargs)
 
     def find(self, *args: Any, **kwargs: Any) -> Cursor[DocumentType]:
         """
         Query the database.
         """
-        return self._get_collection().find(args, kwargs)
+        return self._get_collection().find(*args, **kwargs)
 
     def _get_collection(self, collection_name: Optional[str] = None) -> Collection[DocumentType]:
         return self._mongo_client.get_database(self._database).get_collection(
             collection_name or self._collection
         )
 
     def __repr__(self) -> str:
```

### Comparing `ixoncdkingress-0.0.8/ixoncdkingress/types.py` & `ixoncdkingress-0.0.9/ixoncdkingress/types.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.8/ixoncdkingress/webserver/config.py` & `ixoncdkingress-0.0.9/ixoncdkingress/webserver/config.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.8/ixoncdkingress/webserver/form.py` & `ixoncdkingress-0.0.9/ixoncdkingress/webserver/form.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.8/ixoncdkingress/webserver/request.py` & `ixoncdkingress-0.0.9/ixoncdkingress/webserver/request.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.8/ixoncdkingress/webserver/response.py` & `ixoncdkingress-0.0.9/ixoncdkingress/webserver/response.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.8/ixoncdkingress/webserver/servlet.py` & `ixoncdkingress-0.0.9/ixoncdkingress/webserver/servlet.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.8/ixoncdkingress/webserver/utils.py` & `ixoncdkingress-0.0.9/ixoncdkingress/webserver/utils.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.8/ixoncdkingress/webserver/wsgi.py` & `ixoncdkingress-0.0.9/ixoncdkingress/webserver/wsgi.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.8/ixoncdkingress.egg-info/SOURCES.txt` & `ixoncdkingress-0.0.9/ixoncdkingress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.8/setup.py` & `ixoncdkingress-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     'pytest-mock==3.8.2',
     'types-requests>=2.28.11.5',
     'wouter==0.0.3',
 ]
 
 setup(
     name='ixoncdkingress',
-    version='0.0.8',
+    version='0.0.9',
     description='IXON CDK Ingress used in Custom Backend Components(CBC) for the IXON Cloud',
     author='IXON',
     author_email='development@ixon.cloud',
     url='https://www.ixon.cloud/',
     packages=find_packages(exclude=['tests*', ]),
     package_data={
         '': ['py.typed', 'assets/*'],
```

### Comparing `ixoncdkingress-0.0.8/tests/test___main__.py` & `ixoncdkingress-0.0.9/tests/test___main__.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.8/tests/test_utils.py` & `ixoncdkingress-0.0.9/tests/test_utils.py`

 * *Files identical despite different names*

