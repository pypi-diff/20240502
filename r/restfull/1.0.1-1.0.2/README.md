# Comparing `tmp/restfull-1.0.1.tar.gz` & `tmp/restfull-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restfull-1.0.1.tar", last modified: Thu May  2 16:24:13 2024, max compression
+gzip compressed data, was "restfull-1.0.2.tar", last modified: Thu May  2 17:44:59 2024, max compression
```

## Comparing `restfull-1.0.1.tar` & `restfull-1.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 16:24:13.782671 restfull-1.0.1/
--rw-r--r--   0 michael    (501) staff       (20)      293 2024-05-02 16:23:20.000000 restfull-1.0.1/.bumpversion.cfg
--rw-r--r--   0 michael    (501) staff       (20)     3125 2024-05-01 21:50:19.000000 restfull-1.0.1/.gitignore
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 16:24:13.776410 restfull-1.0.1/.idea/
--rw-r--r--   0 michael    (501) staff       (20)      176 2024-05-01 15:13:54.000000 restfull-1.0.1/.idea/.gitignore
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 16:24:13.777125 restfull-1.0.1/.idea/inspectionProfiles/
--rw-r--r--   0 michael    (501) staff       (20)     4768 2024-05-01 15:13:54.000000 restfull-1.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 michael    (501) staff       (20)      174 2024-05-01 15:13:55.000000 restfull-1.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 michael    (501) staff       (20)      298 2024-05-01 15:21:37.000000 restfull-1.0.1/.idea/misc.xml
--rw-r--r--   0 michael    (501) staff       (20)      268 2024-05-01 15:13:55.000000 restfull-1.0.1/.idea/modules.xml
--rw-r--r--   0 michael    (501) staff       (20)      353 2024-05-01 15:13:55.000000 restfull-1.0.1/.idea/restfull.iml
--rw-r--r--   0 michael    (501) staff       (20)      180 2024-05-01 15:13:55.000000 restfull-1.0.1/.idea/vcs.xml
--rw-r--r--   0 michael    (501) staff       (20)     1074 2024-05-01 21:53:55.000000 restfull-1.0.1/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)      571 2024-05-01 21:46:50.000000 restfull-1.0.1/Makefile
--rw-r--r--   0 michael    (501) staff       (20)      988 2024-05-02 16:24:13.781903 restfull-1.0.1/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)       67 2024-05-02 16:23:20.000000 restfull-1.0.1/README.md
--rw-r--r--   0 michael    (501) staff       (20)        6 2024-05-02 16:23:20.000000 restfull-1.0.1/VERSION
--rw-r--r--   0 michael    (501) staff       (20)      133 2024-05-01 21:34:39.000000 restfull-1.0.1/requirements.txt
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 16:24:13.779194 restfull-1.0.1/restfull/
--rw-r--r--   0 michael    (501) staff       (20)      161 2024-05-02 16:23:20.000000 restfull-1.0.1/restfull/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      256 2024-05-01 19:04:43.000000 restfull-1.0.1/restfull/base_auth.py
--rw-r--r--   0 michael    (501) staff       (20)      632 2024-05-01 19:04:43.000000 restfull-1.0.1/restfull/basic_auth.py
--rw-r--r--   0 michael    (501) staff       (20)      416 2024-05-02 16:18:39.000000 restfull-1.0.1/restfull/bearer_auth.py
--rw-r--r--   0 michael    (501) staff       (20)      689 2024-05-01 19:56:28.000000 restfull-1.0.1/restfull/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)     8123 2024-05-01 22:52:39.000000 restfull-1.0.1/restfull/restapi.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 16:24:13.780223 restfull-1.0.1/restfull.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)      988 2024-05-02 16:24:13.000000 restfull-1.0.1/restfull.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      628 2024-05-02 16:24:13.000000 restfull-1.0.1/restfull.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2024-05-02 16:24:13.000000 restfull-1.0.1/restfull.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       96 2024-05-02 16:24:13.000000 restfull-1.0.1/restfull.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        9 2024-05-02 16:24:13.000000 restfull-1.0.1/restfull.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2024-05-02 16:24:13.782734 restfull-1.0.1/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1274 2024-05-01 22:59:33.000000 restfull-1.0.1/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 16:24:13.781484 restfull-1.0.1/tests/
--rw-r--r--   0 michael    (501) staff       (20)        0 2024-05-01 21:30:18.000000 restfull-1.0.1/tests/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      535 2024-05-01 21:30:54.000000 restfull-1.0.1/tests/conftest.py
--rw-r--r--   0 michael    (501) staff       (20)      101 2024-05-01 21:31:14.000000 restfull-1.0.1/tests/pytest.ini
--rw-r--r--   0 michael    (501) staff       (20)     4087 2024-05-01 22:56:21.000000 restfull-1.0.1/tests/test_1.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 17:44:59.739161 restfull-1.0.2/
+-rw-r--r--   0 michael    (501) staff       (20)      293 2024-05-02 17:44:47.000000 restfull-1.0.2/.bumpversion.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     3125 2024-05-01 21:50:19.000000 restfull-1.0.2/.gitignore
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 17:44:59.726197 restfull-1.0.2/.idea/
+-rw-r--r--   0 michael    (501) staff       (20)      176 2024-05-01 15:13:54.000000 restfull-1.0.2/.idea/.gitignore
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 17:44:59.726863 restfull-1.0.2/.idea/inspectionProfiles/
+-rw-r--r--   0 michael    (501) staff       (20)     4768 2024-05-01 15:13:54.000000 restfull-1.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 michael    (501) staff       (20)      174 2024-05-01 15:13:55.000000 restfull-1.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 michael    (501) staff       (20)      298 2024-05-01 15:21:37.000000 restfull-1.0.2/.idea/misc.xml
+-rw-r--r--   0 michael    (501) staff       (20)      268 2024-05-01 15:13:55.000000 restfull-1.0.2/.idea/modules.xml
+-rw-r--r--   0 michael    (501) staff       (20)      353 2024-05-01 15:13:55.000000 restfull-1.0.2/.idea/restfull.iml
+-rw-r--r--   0 michael    (501) staff       (20)      180 2024-05-01 15:13:55.000000 restfull-1.0.2/.idea/vcs.xml
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2024-05-01 21:53:55.000000 restfull-1.0.2/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)      571 2024-05-01 21:46:50.000000 restfull-1.0.2/Makefile
+-rw-r--r--   0 michael    (501) staff       (20)      988 2024-05-02 17:44:59.731880 restfull-1.0.2/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)       67 2024-05-02 17:44:47.000000 restfull-1.0.2/README.md
+-rw-r--r--   0 michael    (501) staff       (20)        6 2024-05-02 17:44:47.000000 restfull-1.0.2/VERSION
+-rw-r--r--   0 michael    (501) staff       (20)      133 2024-05-01 21:34:39.000000 restfull-1.0.2/requirements.txt
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 17:44:59.729036 restfull-1.0.2/restfull/
+-rw-r--r--   0 michael    (501) staff       (20)      161 2024-05-02 17:44:47.000000 restfull-1.0.2/restfull/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      256 2024-05-01 19:04:43.000000 restfull-1.0.2/restfull/base_auth.py
+-rw-r--r--   0 michael    (501) staff       (20)      632 2024-05-01 19:04:43.000000 restfull-1.0.2/restfull/basic_auth.py
+-rw-r--r--   0 michael    (501) staff       (20)      416 2024-05-02 16:18:39.000000 restfull-1.0.2/restfull/bearer_auth.py
+-rw-r--r--   0 michael    (501) staff       (20)      689 2024-05-01 19:56:28.000000 restfull-1.0.2/restfull/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)     8569 2024-05-02 17:44:30.000000 restfull-1.0.2/restfull/restapi.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 17:44:59.730283 restfull-1.0.2/restfull.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)      988 2024-05-02 17:44:59.000000 restfull-1.0.2/restfull.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      628 2024-05-02 17:44:59.000000 restfull-1.0.2/restfull.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2024-05-02 17:44:59.000000 restfull-1.0.2/restfull.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       96 2024-05-02 17:44:59.000000 restfull-1.0.2/restfull.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        9 2024-05-02 17:44:59.000000 restfull-1.0.2/restfull.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2024-05-02 17:44:59.739210 restfull-1.0.2/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1274 2024-05-01 22:59:33.000000 restfull-1.0.2/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 17:44:59.731425 restfull-1.0.2/tests/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2024-05-01 21:30:18.000000 restfull-1.0.2/tests/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      535 2024-05-01 21:30:54.000000 restfull-1.0.2/tests/conftest.py
+-rw-r--r--   0 michael    (501) staff       (20)      101 2024-05-01 21:31:14.000000 restfull-1.0.2/tests/pytest.ini
+-rw-r--r--   0 michael    (501) staff       (20)     4087 2024-05-01 22:56:21.000000 restfull-1.0.2/tests/test_1.py
```

### Comparing `restfull-1.0.1/.gitignore` & `restfull-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `restfull-1.0.1/.idea/inspectionProfiles/Project_Default.xml` & `restfull-1.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `restfull-1.0.1/LICENSE.txt` & `restfull-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `restfull-1.0.1/Makefile` & `restfull-1.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `restfull-1.0.1/PKG-INFO` & `restfull-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restfull
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python REST API Frontend
 Home-page: https://github.com/mminichino/restfull
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: utilities,rest,api
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,13 +20,13 @@
 License-File: LICENSE.txt
 Requires-Dist: requests>=2.31.0
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: pytoolbase>=1.0.1
 Requires-Dist: python-certifi-win32>=1.6.1
 Requires-Dist: certifi>=2023.5.7
 
-# pytoolbase 1.0.1
+# pytoolbase 1.0.2
 
 ## Installing
 ```
 $ pip install pytoolbase
 ```
```

### Comparing `restfull-1.0.1/restfull/basic_auth.py` & `restfull-1.0.2/restfull/basic_auth.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.1/restfull/exceptions.py` & `restfull-1.0.2/restfull/exceptions.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.1/restfull/restapi.py` & `restfull-1.0.2/restfull/restapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         self.hostname = hostname
         self.auth_class = auth_class
         self.ssl = use_ssl
         self.verify = verify
         self.port = port
         self.scheme = 'https' if self.ssl else 'http'
         self.response_text = None
-        self.response_list = []
         self.response_dict = {}
         self.response_code = 200
         try:
             self.loop = asyncio.get_event_loop()
         except RuntimeError:
             self.loop = asyncio.new_event_loop()
             asyncio.set_event_loop(self.loop)
@@ -151,23 +150,29 @@
             else:
                 self.response_dict = json.loads(self.response_text).get(data_key)
         except (json.decoder.JSONDecodeError, AttributeError):
             self.response_dict = {}
         return self
 
     def filter(self, key: str, value: str):
-        self.response_list = [item for item in self.response_list if item.get(key) == value]
+        if type(self.response_dict) is list:
+            self.response_dict = [item for item in self.response_dict if item.get(key) == value]
+        else:
+            self.response_dict = self.response_dict if dict(self.response_dict).get(key) == value else {}
         return self
 
     def list_item(self, index: int):
         try:
             return list(self.records())[index]
         except IndexError:
             return None
 
+    def list(self):
+        return list(self.records())
+
     def json_key(self, key: str):
         record = self.record()
         return record.get(key)
 
     def records(self):
         if type(self.response_dict) is list:
             for element in self.response_dict:
@@ -184,19 +189,32 @@
         return self.record()
 
     def page_count(self, total_tag: str = "total", pages_tag: str = "total_pages"):
         record = self.record()
         return record.get(total_tag), record.get(pages_tag)
 
     @property
+    def is_present(self) -> bool:
+        if self.response_dict:
+            return True
+        else:
+            return False
+
+    @property
+    def is_empty(self) -> bool:
+        if self.response_dict:
+            return False
+        else:
+            return True
+
+    @property
     def code(self):
         return self.response_code
 
     def reset(self):
-        self.response_list = []
         self.response_dict = {}
 
     @staticmethod
     def paged_endpoint(endpoint: str, page_tag: str = "page", page: int = 1, per_page_tag: Union[str, None] = None, per_page: int = 10) -> str:
         _endpoint = f"{endpoint}?{page_tag}={page}"
         if per_page_tag:
             _endpoint += f"&{per_page_tag}={per_page}"
```

### Comparing `restfull-1.0.1/restfull.egg-info/PKG-INFO` & `restfull-1.0.2/restfull.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restfull
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python REST API Frontend
 Home-page: https://github.com/mminichino/restfull
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: utilities,rest,api
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,13 +20,13 @@
 License-File: LICENSE.txt
 Requires-Dist: requests>=2.31.0
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: pytoolbase>=1.0.1
 Requires-Dist: python-certifi-win32>=1.6.1
 Requires-Dist: certifi>=2023.5.7
 
-# pytoolbase 1.0.1
+# pytoolbase 1.0.2
 
 ## Installing
 ```
 $ pip install pytoolbase
 ```
```

### Comparing `restfull-1.0.1/restfull.egg-info/SOURCES.txt` & `restfull-1.0.2/restfull.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `restfull-1.0.1/setup.py` & `restfull-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.1/tests/conftest.py` & `restfull-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.1/tests/test_1.py` & `restfull-1.0.2/tests/test_1.py`

 * *Files identical despite different names*

