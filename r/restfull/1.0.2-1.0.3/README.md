# Comparing `tmp/restfull-1.0.2.tar.gz` & `tmp/restfull-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restfull-1.0.2.tar", last modified: Thu May  2 17:44:59 2024, max compression
+gzip compressed data, was "restfull-1.0.3.tar", last modified: Thu May  2 18:01:25 2024, max compression
```

## Comparing `restfull-1.0.2.tar` & `restfull-1.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 17:44:59.739161 restfull-1.0.2/
--rw-r--r--   0 michael    (501) staff       (20)      293 2024-05-02 17:44:47.000000 restfull-1.0.2/.bumpversion.cfg
--rw-r--r--   0 michael    (501) staff       (20)     3125 2024-05-01 21:50:19.000000 restfull-1.0.2/.gitignore
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 17:44:59.726197 restfull-1.0.2/.idea/
--rw-r--r--   0 michael    (501) staff       (20)      176 2024-05-01 15:13:54.000000 restfull-1.0.2/.idea/.gitignore
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 17:44:59.726863 restfull-1.0.2/.idea/inspectionProfiles/
--rw-r--r--   0 michael    (501) staff       (20)     4768 2024-05-01 15:13:54.000000 restfull-1.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 michael    (501) staff       (20)      174 2024-05-01 15:13:55.000000 restfull-1.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 michael    (501) staff       (20)      298 2024-05-01 15:21:37.000000 restfull-1.0.2/.idea/misc.xml
--rw-r--r--   0 michael    (501) staff       (20)      268 2024-05-01 15:13:55.000000 restfull-1.0.2/.idea/modules.xml
--rw-r--r--   0 michael    (501) staff       (20)      353 2024-05-01 15:13:55.000000 restfull-1.0.2/.idea/restfull.iml
--rw-r--r--   0 michael    (501) staff       (20)      180 2024-05-01 15:13:55.000000 restfull-1.0.2/.idea/vcs.xml
--rw-r--r--   0 michael    (501) staff       (20)     1074 2024-05-01 21:53:55.000000 restfull-1.0.2/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)      571 2024-05-01 21:46:50.000000 restfull-1.0.2/Makefile
--rw-r--r--   0 michael    (501) staff       (20)      988 2024-05-02 17:44:59.731880 restfull-1.0.2/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)       67 2024-05-02 17:44:47.000000 restfull-1.0.2/README.md
--rw-r--r--   0 michael    (501) staff       (20)        6 2024-05-02 17:44:47.000000 restfull-1.0.2/VERSION
--rw-r--r--   0 michael    (501) staff       (20)      133 2024-05-01 21:34:39.000000 restfull-1.0.2/requirements.txt
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 17:44:59.729036 restfull-1.0.2/restfull/
--rw-r--r--   0 michael    (501) staff       (20)      161 2024-05-02 17:44:47.000000 restfull-1.0.2/restfull/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      256 2024-05-01 19:04:43.000000 restfull-1.0.2/restfull/base_auth.py
--rw-r--r--   0 michael    (501) staff       (20)      632 2024-05-01 19:04:43.000000 restfull-1.0.2/restfull/basic_auth.py
--rw-r--r--   0 michael    (501) staff       (20)      416 2024-05-02 16:18:39.000000 restfull-1.0.2/restfull/bearer_auth.py
--rw-r--r--   0 michael    (501) staff       (20)      689 2024-05-01 19:56:28.000000 restfull-1.0.2/restfull/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)     8569 2024-05-02 17:44:30.000000 restfull-1.0.2/restfull/restapi.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 17:44:59.730283 restfull-1.0.2/restfull.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)      988 2024-05-02 17:44:59.000000 restfull-1.0.2/restfull.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      628 2024-05-02 17:44:59.000000 restfull-1.0.2/restfull.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2024-05-02 17:44:59.000000 restfull-1.0.2/restfull.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       96 2024-05-02 17:44:59.000000 restfull-1.0.2/restfull.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        9 2024-05-02 17:44:59.000000 restfull-1.0.2/restfull.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2024-05-02 17:44:59.739210 restfull-1.0.2/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1274 2024-05-01 22:59:33.000000 restfull-1.0.2/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 17:44:59.731425 restfull-1.0.2/tests/
--rw-r--r--   0 michael    (501) staff       (20)        0 2024-05-01 21:30:18.000000 restfull-1.0.2/tests/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      535 2024-05-01 21:30:54.000000 restfull-1.0.2/tests/conftest.py
--rw-r--r--   0 michael    (501) staff       (20)      101 2024-05-01 21:31:14.000000 restfull-1.0.2/tests/pytest.ini
--rw-r--r--   0 michael    (501) staff       (20)     4087 2024-05-01 22:56:21.000000 restfull-1.0.2/tests/test_1.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:01:25.373137 restfull-1.0.3/
+-rw-r--r--   0 michael    (501) staff       (20)      293 2024-05-02 18:01:17.000000 restfull-1.0.3/.bumpversion.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     3125 2024-05-01 21:50:19.000000 restfull-1.0.3/.gitignore
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:01:25.356940 restfull-1.0.3/.idea/
+-rw-r--r--   0 michael    (501) staff       (20)      176 2024-05-01 15:13:54.000000 restfull-1.0.3/.idea/.gitignore
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:01:25.357836 restfull-1.0.3/.idea/inspectionProfiles/
+-rw-r--r--   0 michael    (501) staff       (20)     4768 2024-05-01 15:13:54.000000 restfull-1.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 michael    (501) staff       (20)      174 2024-05-01 15:13:55.000000 restfull-1.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 michael    (501) staff       (20)      298 2024-05-01 15:21:37.000000 restfull-1.0.3/.idea/misc.xml
+-rw-r--r--   0 michael    (501) staff       (20)      268 2024-05-01 15:13:55.000000 restfull-1.0.3/.idea/modules.xml
+-rw-r--r--   0 michael    (501) staff       (20)      353 2024-05-01 15:13:55.000000 restfull-1.0.3/.idea/restfull.iml
+-rw-r--r--   0 michael    (501) staff       (20)      180 2024-05-01 15:13:55.000000 restfull-1.0.3/.idea/vcs.xml
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2024-05-01 21:53:55.000000 restfull-1.0.3/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)      571 2024-05-01 21:46:50.000000 restfull-1.0.3/Makefile
+-rw-r--r--   0 michael    (501) staff       (20)      984 2024-05-02 18:01:25.362896 restfull-1.0.3/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)       63 2024-05-02 18:01:17.000000 restfull-1.0.3/README.md
+-rw-r--r--   0 michael    (501) staff       (20)        6 2024-05-02 18:01:17.000000 restfull-1.0.3/VERSION
+-rw-r--r--   0 michael    (501) staff       (20)      133 2024-05-01 21:34:39.000000 restfull-1.0.3/requirements.txt
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:01:25.359955 restfull-1.0.3/restfull/
+-rw-r--r--   0 michael    (501) staff       (20)      161 2024-05-02 18:01:17.000000 restfull-1.0.3/restfull/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      256 2024-05-01 19:04:43.000000 restfull-1.0.3/restfull/base_auth.py
+-rw-r--r--   0 michael    (501) staff       (20)      632 2024-05-01 19:04:43.000000 restfull-1.0.3/restfull/basic_auth.py
+-rw-r--r--   0 michael    (501) staff       (20)      416 2024-05-02 16:18:39.000000 restfull-1.0.3/restfull/bearer_auth.py
+-rw-r--r--   0 michael    (501) staff       (20)      689 2024-05-01 19:56:28.000000 restfull-1.0.3/restfull/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)     8569 2024-05-02 17:44:30.000000 restfull-1.0.3/restfull/restapi.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:01:25.361227 restfull-1.0.3/restfull.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)      984 2024-05-02 18:01:25.000000 restfull-1.0.3/restfull.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      628 2024-05-02 18:01:25.000000 restfull-1.0.3/restfull.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2024-05-02 18:01:25.000000 restfull-1.0.3/restfull.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       96 2024-05-02 18:01:25.000000 restfull-1.0.3/restfull.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        9 2024-05-02 18:01:25.000000 restfull-1.0.3/restfull.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2024-05-02 18:01:25.373214 restfull-1.0.3/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1274 2024-05-01 22:59:33.000000 restfull-1.0.3/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 18:01:25.362456 restfull-1.0.3/tests/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2024-05-01 21:30:18.000000 restfull-1.0.3/tests/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      535 2024-05-01 21:30:54.000000 restfull-1.0.3/tests/conftest.py
+-rw-r--r--   0 michael    (501) staff       (20)      101 2024-05-01 21:31:14.000000 restfull-1.0.3/tests/pytest.ini
+-rw-r--r--   0 michael    (501) staff       (20)     4087 2024-05-01 22:56:21.000000 restfull-1.0.3/tests/test_1.py
```

### Comparing `restfull-1.0.2/.gitignore` & `restfull-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `restfull-1.0.2/.idea/inspectionProfiles/Project_Default.xml` & `restfull-1.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `restfull-1.0.2/LICENSE.txt` & `restfull-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `restfull-1.0.2/Makefile` & `restfull-1.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `restfull-1.0.2/PKG-INFO` & `restfull-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restfull
-Version: 1.0.2
+Version: 1.0.3
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
 
-# pytoolbase 1.0.2
+# restfull 1.0.3
 
 ## Installing
 ```
-$ pip install pytoolbase
+$ pip install restfull
 ```
```

### Comparing `restfull-1.0.2/restfull/basic_auth.py` & `restfull-1.0.3/restfull/basic_auth.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.2/restfull/exceptions.py` & `restfull-1.0.3/restfull/exceptions.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.2/restfull/restapi.py` & `restfull-1.0.3/restfull/restapi.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.2/restfull.egg-info/PKG-INFO` & `restfull-1.0.3/restfull.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restfull
-Version: 1.0.2
+Version: 1.0.3
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
 
-# pytoolbase 1.0.2
+# restfull 1.0.3
 
 ## Installing
 ```
-$ pip install pytoolbase
+$ pip install restfull
 ```
```

### Comparing `restfull-1.0.2/restfull.egg-info/SOURCES.txt` & `restfull-1.0.3/restfull.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `restfull-1.0.2/setup.py` & `restfull-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.2/tests/conftest.py` & `restfull-1.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.2/tests/test_1.py` & `restfull-1.0.3/tests/test_1.py`

 * *Files identical despite different names*

