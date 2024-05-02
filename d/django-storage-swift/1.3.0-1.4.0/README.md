# Comparing `tmp/django-storage-swift-1.3.0.tar.gz` & `tmp/django_storage_swift-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-storage-swift-1.3.0.tar", last modified: Thu Jul 27 19:15:39 2023, max compression
+gzip compressed data, was "django_storage_swift-1.4.0.tar", last modified: Thu May  2 12:46:26 2024, max compression
```

## Comparing `django-storage-swift-1.3.0.tar` & `django_storage_swift-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-07-27 19:15:39.473931 django-storage-swift-1.3.0/
--rw-r--r--   0 dennis    (1000) dennis    (1000)     1069 2023-07-27 19:11:23.000000 django-storage-swift-1.3.0/LICENSE.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)       19 2023-07-27 19:11:23.000000 django-storage-swift-1.3.0/MANIFEST.in
--rw-r--r--   0 dennis    (1000) dennis    (1000)    21918 2023-07-27 19:15:39.473931 django-storage-swift-1.3.0/PKG-INFO
--rw-r--r--   0 dennis    (1000) dennis    (1000)    21149 2023-07-27 19:11:23.000000 django-storage-swift-1.3.0/README.rst
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-07-27 19:15:39.473931 django-storage-swift-1.3.0/django_storage_swift.egg-info/
--rw-r--r--   0 dennis    (1000) dennis    (1000)    21918 2023-07-27 19:15:39.000000 django-storage-swift-1.3.0/django_storage_swift.egg-info/PKG-INFO
--rw-r--r--   0 dennis    (1000) dennis    (1000)      365 2023-07-27 19:15:39.000000 django-storage-swift-1.3.0/django_storage_swift.egg-info/SOURCES.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)        1 2023-07-27 19:15:39.000000 django-storage-swift-1.3.0/django_storage_swift.egg-info/dependency_links.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)        1 2023-07-27 19:14:36.000000 django-storage-swift-1.3.0/django_storage_swift.egg-info/not-zip-safe
--rw-r--r--   0 dennis    (1000) dennis    (1000)       80 2023-07-27 19:15:39.000000 django-storage-swift-1.3.0/django_storage_swift.egg-info/requires.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)        6 2023-07-27 19:15:39.000000 django-storage-swift-1.3.0/django_storage_swift.egg-info/top_level.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)       67 2023-07-27 19:15:39.473931 django-storage-swift-1.3.0/setup.cfg
--rw-r--r--   0 dennis    (1000) dennis    (1000)     1060 2023-07-27 19:15:33.000000 django-storage-swift-1.3.0/setup.py
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-07-27 19:15:39.473931 django-storage-swift-1.3.0/swift/
--rw-r--r--   0 dennis    (1000) dennis    (1000)        0 2023-07-27 19:11:23.000000 django-storage-swift-1.3.0/swift/__init__.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)    17316 2023-07-27 19:11:23.000000 django-storage-swift-1.3.0/swift/storage.py
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-07-27 19:15:39.473931 django-storage-swift-1.3.0/tests/
--rw-r--r--   0 dennis    (1000) dennis    (1000)    18611 2023-07-27 19:11:23.000000 django-storage-swift-1.3.0/tests/tests.py
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2024-05-02 12:46:26.912263 django_storage_swift-1.4.0/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     1069 2023-07-27 19:11:23.000000 django_storage_swift-1.4.0/LICENSE.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       19 2023-07-27 19:11:23.000000 django_storage_swift-1.4.0/MANIFEST.in
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    22058 2024-05-02 12:46:26.912263 django_storage_swift-1.4.0/PKG-INFO
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    21149 2023-07-27 19:11:23.000000 django_storage_swift-1.4.0/README.rst
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2024-05-02 12:46:26.912263 django_storage_swift-1.4.0/django_storage_swift.egg-info/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    22058 2024-05-02 12:46:26.000000 django_storage_swift-1.4.0/django_storage_swift.egg-info/PKG-INFO
+-rw-r--r--   0 dennis    (1000) dennis    (1000)      380 2024-05-02 12:46:26.000000 django_storage_swift-1.4.0/django_storage_swift.egg-info/SOURCES.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)        1 2024-05-02 12:46:26.000000 django_storage_swift-1.4.0/django_storage_swift.egg-info/dependency_links.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)        1 2023-07-27 19:14:36.000000 django_storage_swift-1.4.0/django_storage_swift.egg-info/not-zip-safe
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       80 2024-05-02 12:46:26.000000 django_storage_swift-1.4.0/django_storage_swift.egg-info/requires.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)        6 2024-05-02 12:46:26.000000 django_storage_swift-1.4.0/django_storage_swift.egg-info/top_level.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       67 2024-05-02 12:46:26.912263 django_storage_swift-1.4.0/setup.cfg
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     1060 2024-05-02 12:45:07.000000 django_storage_swift-1.4.0/setup.py
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2024-05-02 12:46:26.908929 django_storage_swift-1.4.0/swift/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)        0 2023-07-27 19:11:23.000000 django_storage_swift-1.4.0/swift/__init__.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    17237 2024-03-20 10:19:09.000000 django_storage_swift-1.4.0/swift/storage.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)      111 2024-03-20 10:19:09.000000 django_storage_swift-1.4.0/swift/utils.py
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2024-05-02 12:46:26.908929 django_storage_swift-1.4.0/tests/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    18611 2023-07-27 19:11:23.000000 django_storage_swift-1.4.0/tests/tests.py
```

### Comparing `django-storage-swift-1.3.0/LICENSE.txt` & `django_storage_swift-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-storage-swift-1.3.0/PKG-INFO` & `django_storage_swift-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-storage-swift
-Version: 1.3.0
+Version: 1.4.0
 Summary: OpenStack Swift storage backend for Django
 Home-page: https://github.com/dennisv/django-storage-swift
 Author: Dennis Vermeulen
 Author-email: blacktorn@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -13,14 +13,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 License-File: LICENSE.txt
+Requires-Dist: python-swiftclient>=2.2.0
+Requires-Dist: python-keystoneclient>=0.2.3
+Requires-Dist: six
+Requires-Dist: python-magic>=0.4.10
 
 .. image:: https://img.shields.io/pypi/v/django-storage-swift.svg
     :target: https://pypi.python.org/pypi/django-storage-swift
 
 .. image:: https://travis-ci.org/dennisv/django-storage-swift.svg?branch=master
     :target: https://travis-ci.org/dennisv/django-storage-swift
```

### Comparing `django-storage-swift-1.3.0/README.rst` & `django_storage_swift-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-storage-swift-1.3.0/django_storage_swift.egg-info/PKG-INFO` & `django_storage_swift-1.4.0/django_storage_swift.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-storage-swift
-Version: 1.3.0
+Version: 1.4.0
 Summary: OpenStack Swift storage backend for Django
 Home-page: https://github.com/dennisv/django-storage-swift
 Author: Dennis Vermeulen
 Author-email: blacktorn@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -13,14 +13,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 License-File: LICENSE.txt
+Requires-Dist: python-swiftclient>=2.2.0
+Requires-Dist: python-keystoneclient>=0.2.3
+Requires-Dist: six
+Requires-Dist: python-magic>=0.4.10
 
 .. image:: https://img.shields.io/pypi/v/django-storage-swift.svg
     :target: https://pypi.python.org/pypi/django-storage-swift
 
 .. image:: https://travis-ci.org/dennisv/django-storage-swift.svg?branch=master
     :target: https://travis-ci.org/dennisv/django-storage-swift
```

### Comparing `django-storage-swift-1.3.0/setup.py` & `django_storage_swift-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='django-storage-swift',
-    version='1.3.0',
+    version='1.4.0',
     description='OpenStack Swift storage backend for Django',
     long_description=open('README.rst').read(),
     url='https://github.com/dennisv/django-storage-swift',
     author='Dennis Vermeulen',
     author_email='blacktorn@gmail.com',
     license='MIT',
     packages=['swift'],
```

### Comparing `django-storage-swift-1.3.0/swift/storage.py` & `django_storage_swift-1.4.0/swift/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,37 +4,34 @@
 import re
 from datetime import datetime
 from functools import wraps
 from io import BytesIO, UnsupportedOperation
 from time import time
 
 import magic
-from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.core.files import File
 from django.core.files.storage import Storage
 from six.moves.urllib import parse as urlparse
 
+from swift.utils import setting
+
 try:
     from django.utils.deconstruct import deconstructible
 except ImportError:
     def deconstructible(arg):
         return arg
 
 try:
     import swiftclient
     from swiftclient.utils import generate_temp_url
 except ImportError:
     raise ImproperlyConfigured("Could not load swiftclient library")
 
 
-def setting(name, default=None):
-    return getattr(settings, name, default)
-
-
 def validate_settings(backend):
     # Check mandatory parameters
     if not backend.api_auth_url:
         raise ImproperlyConfigured("The SWIFT_AUTH_URL setting is required")
 
     if not backend.api_username:
         raise ImproperlyConfigured("The SWIFT_USERNAME setting is required")
```

### Comparing `django-storage-swift-1.3.0/tests/tests.py` & `django_storage_swift-1.4.0/tests/tests.py`

 * *Files identical despite different names*

