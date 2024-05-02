# Comparing `tmp/scratchcommunication-2.6.1.tar.gz` & `tmp/scratchcommunication-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-2.6.1.tar", last modified: Fri Apr 26 18:44:18 2024, max compression
+gzip compressed data, was "scratchcommunication-2.7.1.tar", last modified: Thu May  2 16:46:34 2024, max compression
```

## Comparing `scratchcommunication-2.6.1.tar` & `scratchcommunication-2.7.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:44:18.258597 scratchcommunication-2.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16036 2024-04-26 18:44:18.258597 scratchcommunication-2.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15206 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:44:18.254598 scratchcommunication-2.6.1/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/cloud_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:44:18.254598 scratchcommunication-2.6.1/scratchcommunication/cloudrequests/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/cloudrequests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/cloudrequests/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/cloudrequests/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:44:18.258597 scratchcommunication-2.6.1/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16036 2024-04-26 18:44:18.000000 scratchcommunication-2.6.1/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 18:44:18.000000 scratchcommunication-2.6.1/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 18:44:18.000000 scratchcommunication-2.6.1/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-26 18:44:18.000000 scratchcommunication-2.6.1/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-26 18:44:18.000000 scratchcommunication-2.6.1/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:44:18.258597 scratchcommunication-2.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:44:18.258597 scratchcommunication-2.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:46:34.226773 scratchcommunication-2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16430 2024-05-02 16:46:34.226773 scratchcommunication-2.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15570 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:46:34.226773 scratchcommunication-2.7.1/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/cloud_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:46:34.226773 scratchcommunication-2.7.1/scratchcommunication/cloudrequests/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/cloudrequests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/cloudrequests/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/cloudrequests/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:46:34.226773 scratchcommunication-2.7.1/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16430 2024-05-02 16:46:34.000000 scratchcommunication-2.7.1/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-02 16:46:34.000000 scratchcommunication-2.7.1/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:46:34.000000 scratchcommunication-2.7.1/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 16:46:34.000000 scratchcommunication-2.7.1/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 16:46:34.000000 scratchcommunication-2.7.1/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:46:34.226773 scratchcommunication-2.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:46:34.226773 scratchcommunication-2.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/tests/test1.py
```

### Comparing `scratchcommunication-2.6.1/LICENSE` & `scratchcommunication-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.6.1/PKG-INFO` & `scratchcommunication-2.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.6.1
+Version: 2.7.1
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: websocket-client
 Requires-Dist: func-timeout
 Requires-Dist: pycryptodome
 Requires-Dist: attrs
+Requires-Dist: browsercookie
 
 # scratchcommunication
 A python module for communicating with scratch projects
 
 # Installation
 
 Run this in your commandline
@@ -62,14 +63,34 @@
 ```python
 import scratchcommunication
 session = scratchcommunication.Session.login("YOUR_USERNAME", "YOUR_PASSWORD")
 ```
 
 I recommend using your session id instead of your password. 
 
+## Login from browser
+
+This will login using cookies from your browser. It only works if you have that browser installed and if you are logged in.
+
+```python
+import scratchcommunication
+session = scratchcommunication.Session.from_browser(scratchcommunication.ANY)
+```
+
+You can choose from these browsers:
+
+FIREFOX
+CHROME
+EDGE
+SAFARI
+CHROMIUM
+EDGE_DEV
+VIVALDI
+ANY
+
 ## Access account data
 
 Once you have logged into your account, you can access your account data.
 
 ```python
 your_session_id = session.session_id
 your_username = session.username
```

### Comparing `scratchcommunication-2.6.1/README.md` & `scratchcommunication-2.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,34 @@
 ```python
 import scratchcommunication
 session = scratchcommunication.Session.login("YOUR_USERNAME", "YOUR_PASSWORD")
 ```
 
 I recommend using your session id instead of your password. 
 
+## Login from browser
+
+This will login using cookies from your browser. It only works if you have that browser installed and if you are logged in.
+
+```python
+import scratchcommunication
+session = scratchcommunication.Session.from_browser(scratchcommunication.ANY)
+```
+
+You can choose from these browsers:
+
+FIREFOX
+CHROME
+EDGE
+SAFARI
+CHROMIUM
+EDGE_DEV
+VIVALDI
+ANY
+
 ## Access account data
 
 Once you have logged into your account, you can access your account data.
 
 ```python
 your_session_id = session.session_id
 your_username = session.username
```

### Comparing `scratchcommunication-2.6.1/scratchcommunication/cloud.py` & `scratchcommunication-2.7.1/scratchcommunication/cloud.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.6.1/scratchcommunication/cloud_socket.py` & `scratchcommunication-2.7.1/scratchcommunication/cloud_socket.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.6.1/scratchcommunication/cloudrequests/basetypes.py` & `scratchcommunication-2.7.1/scratchcommunication/cloudrequests/basetypes.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.6.1/scratchcommunication/cloudrequests/requests.py` & `scratchcommunication-2.7.1/scratchcommunication/cloudrequests/requests.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.6.1/scratchcommunication/security.py` & `scratchcommunication-2.7.1/scratchcommunication/security.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.6.1/scratchcommunication/session.py` & `scratchcommunication-2.7.1/scratchcommunication/session.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,34 @@
 import warnings
+import requests, json, re
+from typing import Literal, Self, assert_never
 from .headers import headers
-from .exceptions import InvalidValueError, ErrorInCloudSocket
+from .exceptions import InvalidValueError, ErrorInCloudSocket, NotSupported
 from . import cloud, cloud_socket
-import requests, json, re
+try:
+    import browsercookie
+    browsercookie_err = None
+except Exception as e:
+    browsercookie = None
+    browsercookie_err = e
+
+FIREFOX = 0
+CHROME = 1
+EDGE = 2
+SAFARI = 3
+CHROMIUM = 4
+EDGE_DEV = 5
+VIVALDI = 6
+ANY = 7
 
 class Session:
     __slots__ = ("session_id", "username", "headers", "cookies", "xtoken", "email", "id", "permissions", "flags", "banned", "session_data", "mute_status", "new_scratcher")
-    def __init__(self, username : str = None, *, session_id : str):
+    def __init__(self, username : str = None, *, session_id : str = None, _login : bool = False):
+        if not _login:
+            return
         self.session_id = session_id
         self.username = username
         self.headers = headers
         self.cookies = {
             "scratchcsrftoken" : "a",
             "scratchlanguage" : "en",
             "scratchpolicyseen": "true",
@@ -26,20 +44,20 @@
     def __exit__(self, exc_type, exc_value, traceback):
         pass
 
     def logout(self):
         for attr in self.__slots__:
             delattr(self, attr)
 
-    def _login(self):
+    def _login(self, *, _session : requests.Session = None):
         '''
         Don't use this
         '''
         try:
-            account = requests.post("https://scratch.mit.edu/session", headers=self.headers, cookies={
+            account = (_session or requests).post("https://scratch.mit.edu/session", headers=self.headers, cookies={
                 "scratchsessionsid": self.session_id,
                 "scratchcsrftoken": "a",
                 "scratchlanguage": "en",
             }).json()
             self.xtoken = account["user"]["token"]
             self.username = account["user"]["username"]
             self.headers["X-Token"] = self.xtoken
@@ -49,19 +67,63 @@
             self.flags = account["flags"]
             self.banned = account["user"]["banned"]
             self.session_data = account
             self.new_scratcher = account["permissions"]["new_scratcher"]
             self.mute_status = account["permissions"]["mute_status"]
         except Exception:
             if self.username is None:
-                raise ValueError("No username supplied and there was no found. The username is needed.")
+                raise ValueError("No username supplied and there was none found. The username is needed.")
             warnings.warn("Couldn't find token. Most features will probably still work.")
 
     @classmethod
-    def login(cls, username : str, password : str):
+    def from_browser(cls, browser : Literal[0,1,2,3,4,5,6,7]) -> Self:
+        """
+        Import cookies from browser to login
+        """
+        if not browsercookie:
+            raise NotSupported("You cannot use browsercookie") from browsercookie_err
+        match browser:
+            case 0:
+                cookies = browsercookie.firefox()
+            case 1:
+                cookies = browsercookie.chrome()
+            case 2:
+                cookies = browsercookie.edge()
+            case 3:
+                cookies = browsercookie.safari()
+            case 4:
+                cookies = browsercookie.chromium()
+            case 5:
+                cookies = browsercookie.edge_dev()
+            case 6:
+                cookies = browsercookie.vivaldi()
+            case 7:
+                cookies = browsercookie.load()
+            case _:
+                assert_never(browser)
+        
+        with requests.Session() as session:
+            session.cookies.update(cookies)
+            session.headers.update(headers)
+            obj = cls(_login=False)
+            obj.cookies = {
+                "scratchcsrftoken" : "a",
+                "scratchlanguage" : "en",
+                "scratchpolicyseen": "true",
+                "accept": "application/json",
+                "Content-Type": "application/json",
+            }
+            obj.cookies.update(session.cookies.get_dict(".scratch.mit.edu"))
+            obj.session_id = session.cookies.get_dict(".scratch.mit.edu").get("scratchsessionsid")
+            obj.headers = session.headers
+            obj._login(_session=session)
+            return obj
+
+    @classmethod
+    def login(cls, username : str, password : str) -> Self:
         '''
         Login from your username and password.
         '''
         try:
             return cls(
                 username, session_id=str(re.search('"(.*)"', requests.post(
                     "https://scratch.mit.edu/login/",
```

### Comparing `scratchcommunication-2.6.1/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-2.7.1/scratchcommunication.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.6.1
+Version: 2.7.1
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: websocket-client
 Requires-Dist: func-timeout
 Requires-Dist: pycryptodome
 Requires-Dist: attrs
+Requires-Dist: browsercookie
 
 # scratchcommunication
 A python module for communicating with scratch projects
 
 # Installation
 
 Run this in your commandline
@@ -62,14 +63,34 @@
 ```python
 import scratchcommunication
 session = scratchcommunication.Session.login("YOUR_USERNAME", "YOUR_PASSWORD")
 ```
 
 I recommend using your session id instead of your password. 
 
+## Login from browser
+
+This will login using cookies from your browser. It only works if you have that browser installed and if you are logged in.
+
+```python
+import scratchcommunication
+session = scratchcommunication.Session.from_browser(scratchcommunication.ANY)
+```
+
+You can choose from these browsers:
+
+FIREFOX
+CHROME
+EDGE
+SAFARI
+CHROMIUM
+EDGE_DEV
+VIVALDI
+ANY
+
 ## Access account data
 
 Once you have logged into your account, you can access your account data.
 
 ```python
 your_session_id = session.session_id
 your_username = session.username
```

### Comparing `scratchcommunication-2.6.1/scratchcommunication.egg-info/SOURCES.txt` & `scratchcommunication-2.7.1/scratchcommunication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.6.1/setup.py` & `scratchcommunication-2.7.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '2.6.1'
+VERSION = '2.7.1'
 
 setup(
     name='scratchcommunication',
     version=VERSION,
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
@@ -26,11 +26,12 @@
     ],
     keywords=['scratch', 'api'],
     install_requires=[
         'requests',
         'websocket-client',
         'func-timeout',
         'pycryptodome',
-        'attrs'
+        'attrs',
+        'browsercookie'
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.11',
 )
```

### Comparing `scratchcommunication-2.6.1/tests/test1.py` & `scratchcommunication-2.7.1/tests/test1.py`

 * *Files identical despite different names*

