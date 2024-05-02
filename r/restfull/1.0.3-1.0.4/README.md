# Comparing `tmp/restfull-1.0.3.tar.gz` & `tmp/restfull-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restfull-1.0.3.tar", last modified: Thu May  2 18:01:25 2024, max compression
+gzip compressed data, was "restfull-1.0.4.tar", last modified: Thu May  2 18:45:48 2024, max compression
```

## Comparing `restfull-1.0.3.tar` & `restfull-1.0.4.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:01:25.373137 restfull-1.0.3/
--rw-r--r--   0 michael    (501) staff       (20)      293 2024-05-02 18:01:17.000000 restfull-1.0.3/.bumpversion.cfg
--rw-r--r--   0 michael    (501) staff       (20)     3125 2024-05-01 21:50:19.000000 restfull-1.0.3/.gitignore
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:01:25.356940 restfull-1.0.3/.idea/
--rw-r--r--   0 michael    (501) staff       (20)      176 2024-05-01 15:13:54.000000 restfull-1.0.3/.idea/.gitignore
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:01:25.357836 restfull-1.0.3/.idea/inspectionProfiles/
--rw-r--r--   0 michael    (501) staff       (20)     4768 2024-05-01 15:13:54.000000 restfull-1.0.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 michael    (501) staff       (20)      174 2024-05-01 15:13:55.000000 restfull-1.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 michael    (501) staff       (20)      298 2024-05-01 15:21:37.000000 restfull-1.0.3/.idea/misc.xml
--rw-r--r--   0 michael    (501) staff       (20)      268 2024-05-01 15:13:55.000000 restfull-1.0.3/.idea/modules.xml
--rw-r--r--   0 michael    (501) staff       (20)      353 2024-05-01 15:13:55.000000 restfull-1.0.3/.idea/restfull.iml
--rw-r--r--   0 michael    (501) staff       (20)      180 2024-05-01 15:13:55.000000 restfull-1.0.3/.idea/vcs.xml
--rw-r--r--   0 michael    (501) staff       (20)     1074 2024-05-01 21:53:55.000000 restfull-1.0.3/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)      571 2024-05-01 21:46:50.000000 restfull-1.0.3/Makefile
--rw-r--r--   0 michael    (501) staff       (20)      984 2024-05-02 18:01:25.362896 restfull-1.0.3/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)       63 2024-05-02 18:01:17.000000 restfull-1.0.3/README.md
--rw-r--r--   0 michael    (501) staff       (20)        6 2024-05-02 18:01:17.000000 restfull-1.0.3/VERSION
--rw-r--r--   0 michael    (501) staff       (20)      133 2024-05-01 21:34:39.000000 restfull-1.0.3/requirements.txt
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:01:25.359955 restfull-1.0.3/restfull/
--rw-r--r--   0 michael    (501) staff       (20)      161 2024-05-02 18:01:17.000000 restfull-1.0.3/restfull/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      256 2024-05-01 19:04:43.000000 restfull-1.0.3/restfull/base_auth.py
--rw-r--r--   0 michael    (501) staff       (20)      632 2024-05-01 19:04:43.000000 restfull-1.0.3/restfull/basic_auth.py
--rw-r--r--   0 michael    (501) staff       (20)      416 2024-05-02 16:18:39.000000 restfull-1.0.3/restfull/bearer_auth.py
--rw-r--r--   0 michael    (501) staff       (20)      689 2024-05-01 19:56:28.000000 restfull-1.0.3/restfull/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)     8569 2024-05-02 17:44:30.000000 restfull-1.0.3/restfull/restapi.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:01:25.361227 restfull-1.0.3/restfull.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)      984 2024-05-02 18:01:25.000000 restfull-1.0.3/restfull.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      628 2024-05-02 18:01:25.000000 restfull-1.0.3/restfull.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2024-05-02 18:01:25.000000 restfull-1.0.3/restfull.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       96 2024-05-02 18:01:25.000000 restfull-1.0.3/restfull.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        9 2024-05-02 18:01:25.000000 restfull-1.0.3/restfull.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2024-05-02 18:01:25.373214 restfull-1.0.3/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1274 2024-05-01 22:59:33.000000 restfull-1.0.3/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:01:25.362456 restfull-1.0.3/tests/
--rw-r--r--   0 michael    (501) staff       (20)        0 2024-05-01 21:30:18.000000 restfull-1.0.3/tests/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      535 2024-05-01 21:30:54.000000 restfull-1.0.3/tests/conftest.py
--rw-r--r--   0 michael    (501) staff       (20)      101 2024-05-01 21:31:14.000000 restfull-1.0.3/tests/pytest.ini
--rw-r--r--   0 michael    (501) staff       (20)     4087 2024-05-01 22:56:21.000000 restfull-1.0.3/tests/test_1.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:45:48.380692 restfull-1.0.4/
+-rw-r--r--   0 michael    (501) staff       (20)      293 2024-05-02 18:45:40.000000 restfull-1.0.4/.bumpversion.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     3125 2024-05-01 21:50:19.000000 restfull-1.0.4/.gitignore
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:45:48.360401 restfull-1.0.4/.idea/
+-rw-r--r--   0 michael    (501) staff       (20)      176 2024-05-01 15:13:54.000000 restfull-1.0.4/.idea/.gitignore
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:45:48.365505 restfull-1.0.4/.idea/inspectionProfiles/
+-rw-r--r--   0 michael    (501) staff       (20)     4768 2024-05-01 15:13:54.000000 restfull-1.0.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 michael    (501) staff       (20)      174 2024-05-01 15:13:55.000000 restfull-1.0.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 michael    (501) staff       (20)      298 2024-05-01 15:21:37.000000 restfull-1.0.4/.idea/misc.xml
+-rw-r--r--   0 michael    (501) staff       (20)      268 2024-05-01 15:13:55.000000 restfull-1.0.4/.idea/modules.xml
+-rw-r--r--   0 michael    (501) staff       (20)      353 2024-05-01 15:13:55.000000 restfull-1.0.4/.idea/restfull.iml
+-rw-r--r--   0 michael    (501) staff       (20)      180 2024-05-01 15:13:55.000000 restfull-1.0.4/.idea/vcs.xml
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2024-05-01 21:53:55.000000 restfull-1.0.4/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)      571 2024-05-01 21:46:50.000000 restfull-1.0.4/Makefile
+-rw-r--r--   0 michael    (501) staff       (20)     1013 2024-05-02 18:45:48.379690 restfull-1.0.4/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)       63 2024-05-02 18:45:40.000000 restfull-1.0.4/README.md
+-rw-r--r--   0 michael    (501) staff       (20)        6 2024-05-02 18:45:40.000000 restfull-1.0.4/VERSION
+-rw-r--r--   0 michael    (501) staff       (20)      147 2024-05-02 18:24:04.000000 restfull-1.0.4/requirements.txt
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:45:48.373809 restfull-1.0.4/restfull/
+-rw-r--r--   0 michael    (501) staff       (20)      161 2024-05-02 18:45:40.000000 restfull-1.0.4/restfull/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      256 2024-05-01 19:04:43.000000 restfull-1.0.4/restfull/base_auth.py
+-rw-r--r--   0 michael    (501) staff       (20)      632 2024-05-01 19:04:43.000000 restfull-1.0.4/restfull/basic_auth.py
+-rw-r--r--   0 michael    (501) staff       (20)      416 2024-05-02 16:18:39.000000 restfull-1.0.4/restfull/bearer_auth.py
+-rw-r--r--   0 michael    (501) staff       (20)      855 2024-05-02 18:37:18.000000 restfull-1.0.4/restfull/data.py
+-rw-r--r--   0 michael    (501) staff       (20)      689 2024-05-01 19:56:28.000000 restfull-1.0.4/restfull/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)     8805 2024-05-02 18:35:53.000000 restfull-1.0.4/restfull/restapi.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:45:48.375222 restfull-1.0.4/restfull.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1013 2024-05-02 18:45:48.000000 restfull-1.0.4/restfull.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      645 2024-05-02 18:45:48.000000 restfull-1.0.4/restfull.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2024-05-02 18:45:48.000000 restfull-1.0.4/restfull.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)      110 2024-05-02 18:45:48.000000 restfull-1.0.4/restfull.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        9 2024-05-02 18:45:48.000000 restfull-1.0.4/restfull.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2024-05-02 18:45:48.380774 restfull-1.0.4/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1299 2024-05-02 18:24:04.000000 restfull-1.0.4/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:45:48.378988 restfull-1.0.4/tests/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2024-05-01 21:30:18.000000 restfull-1.0.4/tests/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      535 2024-05-01 21:30:54.000000 restfull-1.0.4/tests/conftest.py
+-rw-r--r--   0 michael    (501) staff       (20)      101 2024-05-01 21:31:14.000000 restfull-1.0.4/tests/pytest.ini
+-rw-r--r--   0 michael    (501) staff       (20)     4087 2024-05-01 22:56:21.000000 restfull-1.0.4/tests/test_1.py
```

### Comparing `restfull-1.0.3/.gitignore` & `restfull-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `restfull-1.0.3/.idea/inspectionProfiles/Project_Default.xml` & `restfull-1.0.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `restfull-1.0.3/LICENSE.txt` & `restfull-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `restfull-1.0.3/Makefile` & `restfull-1.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `restfull-1.0.3/PKG-INFO` & `restfull-1.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restfull
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python REST API Frontend
 Home-page: https://github.com/mminichino/restfull
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: utilities,rest,api
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,19 +14,20 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: attrs>=23.1.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: pytoolbase>=1.0.1
 Requires-Dist: python-certifi-win32>=1.6.1
 Requires-Dist: certifi>=2023.5.7
 
-# restfull 1.0.3
+# restfull 1.0.4
 
 ## Installing
 ```
 $ pip install restfull
 ```
```

### Comparing `restfull-1.0.3/restfull/basic_auth.py` & `restfull-1.0.4/restfull/basic_auth.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.3/restfull/exceptions.py` & `restfull-1.0.4/restfull/exceptions.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.3/restfull/restapi.py` & `restfull-1.0.4/restfull/restapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 import json
 import requests
 import warnings
 import asyncio
 import ssl
 from restfull.base_auth import RestAuthBase
+from restfull.data import JsonObject, JsonList
 from typing import Union
 from requests.adapters import HTTPAdapter, Retry
 from aiohttp import ClientSession, TCPConnector
 from pytoolbase.retry import retry
 from pytoolbase.exceptions import NonFatalError
 if os.name == 'nt':
     import certifi_win32
@@ -47,15 +48,15 @@
         self.hostname = hostname
         self.auth_class = auth_class
         self.ssl = use_ssl
         self.verify = verify
         self.port = port
         self.scheme = 'https' if self.ssl else 'http'
         self.response_text = None
-        self.response_dict = {}
+        self.response_dict: Union[list, dict] = {}
         self.response_code = 200
         try:
             self.loop = asyncio.get_event_loop()
         except RuntimeError:
             self.loop = asyncio.new_event_loop()
             asyncio.set_event_loop(self.loop)
 
@@ -188,14 +189,20 @@
             raise ValueError("More than one object matches search criteria")
         return self.record()
 
     def page_count(self, total_tag: str = "total", pages_tag: str = "total_pages"):
         record = self.record()
         return record.get(total_tag), record.get(pages_tag)
 
+    def json_object(self) -> JsonObject:
+        return JsonObject(self.response_dict)
+
+    def json_list(self) -> JsonList:
+        return JsonList(self.response_dict)
+
     @property
     def is_present(self) -> bool:
         if self.response_dict:
             return True
         else:
             return False
```

### Comparing `restfull-1.0.3/restfull.egg-info/PKG-INFO` & `restfull-1.0.4/restfull.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restfull
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python REST API Frontend
 Home-page: https://github.com/mminichino/restfull
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: utilities,rest,api
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,19 +14,20 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: attrs>=23.1.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: pytoolbase>=1.0.1
 Requires-Dist: python-certifi-win32>=1.6.1
 Requires-Dist: certifi>=2023.5.7
 
-# restfull 1.0.3
+# restfull 1.0.4
 
 ## Installing
 ```
 $ pip install restfull
 ```
```

### Comparing `restfull-1.0.3/restfull.egg-info/SOURCES.txt` & `restfull-1.0.4/restfull.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 .idea/vcs.xml
 .idea/inspectionProfiles/Project_Default.xml
 .idea/inspectionProfiles/profiles_settings.xml
 restfull/__init__.py
 restfull/base_auth.py
 restfull/basic_auth.py
 restfull/bearer_auth.py
+restfull/data.py
 restfull/exceptions.py
 restfull/restapi.py
 restfull.egg-info/PKG-INFO
 restfull.egg-info/SOURCES.txt
 restfull.egg-info/dependency_links.txt
 restfull.egg-info/requires.txt
 restfull.egg-info/top_level.txt
```

### Comparing `restfull-1.0.3/setup.py` & `restfull-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     version=restfull.__version__,
     packages=find_packages(exclude=['tests']),
     url='https://github.com/mminichino/restfull',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.8',
     install_requires=[
+        "attrs>=23.1.0",
         "requests>=2.31.0",
         "aiohttp>=3.9.3",
         "pytoolbase>=1.0.1",
         "python-certifi-win32>=1.6.1",
         "certifi>=2023.5.7"
     ],
     author_email='info@unix.us.com',
```

### Comparing `restfull-1.0.3/tests/conftest.py` & `restfull-1.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.3/tests/test_1.py` & `restfull-1.0.4/tests/test_1.py`

 * *Files identical despite different names*

