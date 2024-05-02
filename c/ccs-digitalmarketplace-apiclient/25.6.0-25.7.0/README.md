# Comparing `tmp/ccs-digitalmarketplace-apiclient-25.6.0.tar.gz` & `tmp/ccs-digitalmarketplace-apiclient-25.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-apiclient-25.6.0.tar", last modified: Tue Apr 16 14:26:34 2024, max compression
+gzip compressed data, was "ccs-digitalmarketplace-apiclient-25.7.0.tar", last modified: Thu May  2 12:52:01 2024, max compression
```

## Comparing `ccs-digitalmarketplace-apiclient-25.6.0.tar` & `ccs-digitalmarketplace-apiclient-25.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:26:34.969182 ccs-digitalmarketplace-apiclient-25.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-16 14:26:25.000000 ccs-digitalmarketplace-apiclient-25.6.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-16 14:26:34.969182 ccs-digitalmarketplace-apiclient-25.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-16 14:26:25.000000 ccs-digitalmarketplace-apiclient-25.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:26:34.969182 ccs-digitalmarketplace-apiclient-25.6.0/ccs_digitalmarketplace_apiclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-16 14:26:34.000000 ccs-digitalmarketplace-apiclient-25.6.0/ccs_digitalmarketplace_apiclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-16 14:26:34.000000 ccs-digitalmarketplace-apiclient-25.6.0/ccs_digitalmarketplace_apiclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:26:34.000000 ccs-digitalmarketplace-apiclient-25.6.0/ccs_digitalmarketplace_apiclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 14:26:34.000000 ccs-digitalmarketplace-apiclient-25.6.0/ccs_digitalmarketplace_apiclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 14:26:34.000000 ccs-digitalmarketplace-apiclient-25.6.0/ccs_digitalmarketplace_apiclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:26:34.969182 ccs-digitalmarketplace-apiclient-25.6.0/dmapiclient/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-16 14:26:25.000000 ccs-digitalmarketplace-apiclient-25.6.0/dmapiclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-16 14:26:25.000000 ccs-digitalmarketplace-apiclient-25.6.0/dmapiclient/antivirus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-16 14:26:25.000000 ccs-digitalmarketplace-apiclient-25.6.0/dmapiclient/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-04-16 14:26:25.000000 ccs-digitalmarketplace-apiclient-25.6.0/dmapiclient/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    47189 2024-04-16 14:26:25.000000 ccs-digitalmarketplace-apiclient-25.6.0/dmapiclient/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-16 14:26:25.000000 ccs-digitalmarketplace-apiclient-25.6.0/dmapiclient/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-16 14:26:25.000000 ccs-digitalmarketplace-apiclient-25.6.0/dmapiclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-16 14:26:25.000000 ccs-digitalmarketplace-apiclient-25.6.0/dmapiclient/search.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-16 14:26:34.973182 ccs-digitalmarketplace-apiclient-25.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-16 14:26:25.000000 ccs-digitalmarketplace-apiclient-25.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:52:01.933524 ccs-digitalmarketplace-apiclient-25.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-02 12:51:51.000000 ccs-digitalmarketplace-apiclient-25.7.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 12:52:01.933524 ccs-digitalmarketplace-apiclient-25.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-02 12:51:51.000000 ccs-digitalmarketplace-apiclient-25.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:52:01.933524 ccs-digitalmarketplace-apiclient-25.7.0/ccs_digitalmarketplace_apiclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 12:52:01.000000 ccs-digitalmarketplace-apiclient-25.7.0/ccs_digitalmarketplace_apiclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-02 12:52:01.000000 ccs-digitalmarketplace-apiclient-25.7.0/ccs_digitalmarketplace_apiclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:52:01.000000 ccs-digitalmarketplace-apiclient-25.7.0/ccs_digitalmarketplace_apiclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 12:52:01.000000 ccs-digitalmarketplace-apiclient-25.7.0/ccs_digitalmarketplace_apiclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 12:52:01.000000 ccs-digitalmarketplace-apiclient-25.7.0/ccs_digitalmarketplace_apiclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:52:01.933524 ccs-digitalmarketplace-apiclient-25.7.0/dmapiclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-02 12:51:51.000000 ccs-digitalmarketplace-apiclient-25.7.0/dmapiclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-02 12:51:51.000000 ccs-digitalmarketplace-apiclient-25.7.0/dmapiclient/antivirus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-02 12:51:51.000000 ccs-digitalmarketplace-apiclient-25.7.0/dmapiclient/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-05-02 12:51:51.000000 ccs-digitalmarketplace-apiclient-25.7.0/dmapiclient/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47459 2024-05-02 12:51:51.000000 ccs-digitalmarketplace-apiclient-25.7.0/dmapiclient/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-02 12:51:51.000000 ccs-digitalmarketplace-apiclient-25.7.0/dmapiclient/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 12:51:51.000000 ccs-digitalmarketplace-apiclient-25.7.0/dmapiclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-05-02 12:51:51.000000 ccs-digitalmarketplace-apiclient-25.7.0/dmapiclient/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-02 12:52:01.933524 ccs-digitalmarketplace-apiclient-25.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-02 12:51:51.000000 ccs-digitalmarketplace-apiclient-25.7.0/setup.py
```

### Comparing `ccs-digitalmarketplace-apiclient-25.6.0/LICENCE` & `ccs-digitalmarketplace-apiclient-25.7.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.6.0/README.md` & `ccs-digitalmarketplace-apiclient-25.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.6.0/dmapiclient/antivirus.py` & `ccs-digitalmarketplace-apiclient-25.7.0/dmapiclient/antivirus.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.6.0/dmapiclient/audit.py` & `ccs-digitalmarketplace-apiclient-25.7.0/dmapiclient/audit.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.6.0/dmapiclient/base.py` & `ccs-digitalmarketplace-apiclient-25.7.0/dmapiclient/base.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.6.0/dmapiclient/data.py` & `ccs-digitalmarketplace-apiclient-25.7.0/dmapiclient/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1303,28 +1303,36 @@
     def find_communications(
         self,
         framework,
         supplier_id=None,
         latest_message_target=None,
         archived=None,
         page=None,
-        subject=None
+        subject=None,
+        supplier_name=None,
+        message_text=None,
+        sort_by=None,
+        sort_direction=None
     ):
         warnings.warn(
             "The output of 'find_communications' is paginated. Use 'find_communications_iter' instead.",
             DeprecationWarning
         )
 
         params = {
             'page': page,
             'framework': framework,
             'supplier_id': supplier_id,
             'latest_message_target': latest_message_target,
             'archived': archived,
-            'subject': subject
+            'subject': subject,
+            'supplier_name': supplier_name,
+            'message_text': message_text,
+            'sort_by': sort_by,
+            'sort_direction': sort_direction
         }
 
         return self._get("/communications", params=params)
 
     find_communications_iter = make_iter_method('find_communications', 'communications')
     find_communications_iter.__name__ = str("find_communications_iter")
```

### Comparing `ccs-digitalmarketplace-apiclient-25.6.0/dmapiclient/errors.py` & `ccs-digitalmarketplace-apiclient-25.7.0/dmapiclient/errors.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.6.0/dmapiclient/search.py` & `ccs-digitalmarketplace-apiclient-25.7.0/dmapiclient/search.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.6.0/setup.py` & `ccs-digitalmarketplace-apiclient-25.7.0/setup.py`

 * *Files identical despite different names*

