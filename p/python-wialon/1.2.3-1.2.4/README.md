# Comparing `tmp/python-wialon-1.2.3.tar.gz` & `tmp/python-wialon-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-wialon-1.2.3.tar", last modified: Thu Jan 18 08:03:25 2024, max compression
+gzip compressed data, was "python-wialon-1.2.4.tar", last modified: Thu May  2 11:51:44 2024, max compression
```

## Comparing `python-wialon-1.2.3.tar` & `python-wialon-1.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 niel      (1000) niel      (1000)        0 2024-01-18 08:03:25.803441 python-wialon-1.2.3/
--rw-rw-r--   0 niel      (1000) niel      (1000)     1088 2024-01-18 07:54:02.000000 python-wialon-1.2.3/LICENSE
--rw-rw-r--   0 niel      (1000) niel      (1000)       25 2024-01-18 07:54:02.000000 python-wialon-1.2.3/MANIFEST.in
--rw-r--r--   0 niel      (1000) niel      (1000)     1543 2024-01-18 08:03:25.803441 python-wialon-1.2.3/PKG-INFO
--rw-rw-r--   0 niel      (1000) niel      (1000)      790 2024-01-18 07:54:02.000000 python-wialon-1.2.3/README.md
-drwxrwxr-x   0 niel      (1000) niel      (1000)        0 2024-01-18 08:03:25.803441 python-wialon-1.2.3/python_wialon.egg-info/
--rw-r--r--   0 niel      (1000) niel      (1000)     1543 2024-01-18 08:03:25.000000 python-wialon-1.2.3/python_wialon.egg-info/PKG-INFO
--rw-rw-r--   0 niel      (1000) niel      (1000)      303 2024-01-18 08:03:25.000000 python-wialon-1.2.3/python_wialon.egg-info/SOURCES.txt
--rw-rw-r--   0 niel      (1000) niel      (1000)        1 2024-01-18 08:03:25.000000 python-wialon-1.2.3/python_wialon.egg-info/dependency_links.txt
--rw-rw-r--   0 niel      (1000) niel      (1000)       18 2024-01-18 08:03:25.000000 python-wialon-1.2.3/python_wialon.egg-info/requires.txt
--rw-rw-r--   0 niel      (1000) niel      (1000)       21 2024-01-18 08:03:25.000000 python-wialon-1.2.3/python_wialon.egg-info/top_level.txt
--rw-rw-r--   0 niel      (1000) niel      (1000)        1 2024-01-18 07:54:54.000000 python-wialon-1.2.3/python_wialon.egg-info/zip-safe
--rw-rw-r--   0 niel      (1000) niel      (1000)       38 2024-01-18 08:03:25.803441 python-wialon-1.2.3/setup.cfg
--rw-rw-r--   0 niel      (1000) niel      (1000)     1168 2024-01-18 07:54:02.000000 python-wialon-1.2.3/setup.py
-drwxrwxr-x   0 niel      (1000) niel      (1000)        0 2024-01-18 08:03:25.803441 python-wialon-1.2.3/wialon/
--rw-rw-r--   0 niel      (1000) niel      (1000)      416 2024-01-18 07:55:28.000000 python-wialon-1.2.3/wialon/__init__.py
--rw-rw-r--   0 niel      (1000) niel      (1000)     6920 2024-01-18 07:54:02.000000 python-wialon-1.2.3/wialon/api.py
--rw-rw-r--   0 niel      (1000) niel      (1000)     5210 2024-01-18 07:54:02.000000 python-wialon-1.2.3/wialon/flags.py
+drwxrwxr-x   0 niel      (1000) niel      (1000)        0 2024-05-02 11:51:44.173781 python-wialon-1.2.4/
+-rw-rw-r--   0 niel      (1000) niel      (1000)     1088 2024-01-18 07:54:02.000000 python-wialon-1.2.4/LICENSE
+-rw-rw-r--   0 niel      (1000) niel      (1000)       25 2024-01-18 07:54:02.000000 python-wialon-1.2.4/MANIFEST.in
+-rw-r--r--   0 niel      (1000) niel      (1000)     1543 2024-05-02 11:51:44.173781 python-wialon-1.2.4/PKG-INFO
+-rw-rw-r--   0 niel      (1000) niel      (1000)      790 2024-01-18 07:54:02.000000 python-wialon-1.2.4/README.md
+drwxrwxr-x   0 niel      (1000) niel      (1000)        0 2024-05-02 11:51:44.173781 python-wialon-1.2.4/python_wialon.egg-info/
+-rw-r--r--   0 niel      (1000) niel      (1000)     1543 2024-05-02 11:51:44.000000 python-wialon-1.2.4/python_wialon.egg-info/PKG-INFO
+-rw-rw-r--   0 niel      (1000) niel      (1000)      303 2024-05-02 11:51:44.000000 python-wialon-1.2.4/python_wialon.egg-info/SOURCES.txt
+-rw-rw-r--   0 niel      (1000) niel      (1000)        1 2024-05-02 11:51:44.000000 python-wialon-1.2.4/python_wialon.egg-info/dependency_links.txt
+-rw-rw-r--   0 niel      (1000) niel      (1000)       18 2024-05-02 11:51:44.000000 python-wialon-1.2.4/python_wialon.egg-info/requires.txt
+-rw-rw-r--   0 niel      (1000) niel      (1000)       21 2024-05-02 11:51:44.000000 python-wialon-1.2.4/python_wialon.egg-info/top_level.txt
+-rw-rw-r--   0 niel      (1000) niel      (1000)        1 2024-01-18 07:54:54.000000 python-wialon-1.2.4/python_wialon.egg-info/zip-safe
+-rw-rw-r--   0 niel      (1000) niel      (1000)       38 2024-05-02 11:51:44.173781 python-wialon-1.2.4/setup.cfg
+-rw-rw-r--   0 niel      (1000) niel      (1000)     1168 2024-01-18 07:54:02.000000 python-wialon-1.2.4/setup.py
+drwxrwxr-x   0 niel      (1000) niel      (1000)        0 2024-05-02 11:51:44.173781 python-wialon-1.2.4/wialon/
+-rw-rw-r--   0 niel      (1000) niel      (1000)      416 2024-05-02 11:47:22.000000 python-wialon-1.2.4/wialon/__init__.py
+-rw-rw-r--   0 niel      (1000) niel      (1000)     6921 2024-05-02 11:47:07.000000 python-wialon-1.2.4/wialon/api.py
+-rw-rw-r--   0 niel      (1000) niel      (1000)     5518 2024-05-02 11:47:07.000000 python-wialon-1.2.4/wialon/flags.py
```

### Comparing `python-wialon-1.2.3/LICENSE` & `python-wialon-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-wialon-1.2.3/PKG-INFO` & `python-wialon-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-wialon
-Version: 1.2.3
+Version: 1.2.4
 Summary: Wialon Remote API wrapper for Python.
 Home-page: https://github.com/wialon/python-wialon
 Download-URL: http://pypi.python.org/pypi/python-wialon/
 Author: Alex Chernetsky chal@gurtam.com
 Keywords: wialon remote api wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `python-wialon-1.2.3/README.md` & `python-wialon-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `python-wialon-1.2.3/python_wialon.egg-info/PKG-INFO` & `python-wialon-1.2.4/python_wialon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-wialon
-Version: 1.2.3
+Version: 1.2.4
 Summary: Wialon Remote API wrapper for Python.
 Home-page: https://github.com/wialon/python-wialon
 Download-URL: http://pypi.python.org/pypi/python-wialon/
 Author: Alex Chernetsky chal@gurtam.com
 Keywords: wialon remote api wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `python-wialon-1.2.3/setup.py` & `python-wialon-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `python-wialon-1.2.3/wialon/api.py` & `python-wialon-1.2.4/wialon/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     """
     errors = {
         1: 'Invalid session',
         2: 'Invalid service',
         3: 'Invalid result',
         4: 'Invalid input',
         5: 'Error performing request',
-        6: 'Unknow error',
+        6: 'Unknown error',
         7: 'Access denied',
         8: 'Invalid user name or password',
         9: 'Authorization server is unavailable, please try again later',
         1001: 'No message for selected interval',
         1002: 'Item with such unique property already exists',
         1003: 'Only one request of given time is allowed at the moment'
     }
```

### Comparing `python-wialon-1.2.3/wialon/flags.py` & `python-wialon-1.2.4/wialon/flags.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,17 +104,25 @@
 # Unit commands
 ITEM_UNIT_DATAFLAG_COMMANDS = 0x00000200
 # Unit commands aliases
 ITEM_UNIT_DATAFLAG_COMMAND_ALIASES = 0x00080000
 # TODO
 
 """ User flags """
-#
+# User disabled
+ITEM_USER_USERFLAG_DISABLED = 0x00000001
+# User cannot change password
+ITEM_USER_USERFLAG_CANNOT_CHANGE_PASSWORD = 0x00000002
+# User can create items
 ITEM_USER_USERFLAG_CAN_CREATE_ITEMS = 0x00000004
-# TODO
+# User cannot change settings
+ITEM_USER_USERFLAG_CANNOT_CHANGE_SETTINGS = 0x00000010
+# User can send sms
+ITEM_USER_USERFLAG_CAN_SEND_SMS = 0x00000020
+
 
 """ Item ACL flags """
 # User has at least view access to given item
 ITEM_ACCESSFLAG_VIEW = 0x1
 
 """ Resource ACL flags """
 # View notification
```

